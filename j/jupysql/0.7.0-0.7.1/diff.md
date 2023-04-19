# Comparing `tmp/jupysql-0.7.0.tar.gz` & `tmp/jupysql-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupysql-0.7.0.tar", last modified: Wed Apr  5 15:53:32 2023, max compression
+gzip compressed data, was "jupysql-0.7.1.tar", last modified: Wed Apr 19 17:09:32 2023, max compression
```

## Comparing `jupysql-0.7.0.tar` & `jupysql-0.7.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-05 15:53:32.413157 jupysql-0.7.0/
--rw-r--r--   0 eduardo    (501) staff       (20)    11820 2023-03-30 15:02:40.000000 jupysql-0.7.0/LICENSE
--rw-r--r--   0 eduardo    (501) staff       (20)       52 2022-12-22 14:07:08.000000 jupysql-0.7.0/MANIFEST.in
--rw-r--r--   0 eduardo    (501) staff       (20)     2966 2023-04-05 15:53:32.413208 jupysql-0.7.0/PKG-INFO
--rw-r--r--   0 eduardo    (501) staff       (20)     2303 2023-03-30 15:02:40.000000 jupysql-0.7.0/README.md
--rw-r--r--   0 eduardo    (501) staff       (20)      647 2023-03-30 15:02:40.000000 jupysql-0.7.0/pyproject.toml
--rw-r--r--   0 eduardo    (501) staff       (20)      120 2023-04-05 15:53:32.413388 jupysql-0.7.0/setup.cfg
--rw-r--r--   0 eduardo    (501) staff       (20)     2113 2023-04-05 02:23:57.000000 jupysql-0.7.0/setup.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-05 15:53:32.409154 jupysql-0.7.0/src/
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-05 15:53:32.410586 jupysql-0.7.0/src/jupysql.egg-info/
--rw-r--r--   0 eduardo    (501) staff       (20)     2966 2023-04-05 15:53:32.000000 jupysql-0.7.0/src/jupysql.egg-info/PKG-INFO
--rw-r--r--   0 eduardo    (501) staff       (20)      796 2023-04-05 15:53:32.000000 jupysql-0.7.0/src/jupysql.egg-info/SOURCES.txt
--rw-r--r--   0 eduardo    (501) staff       (20)        1 2023-04-05 15:53:32.000000 jupysql-0.7.0/src/jupysql.egg-info/dependency_links.txt
--rw-r--r--   0 eduardo    (501) staff       (20)        1 2022-12-22 14:07:34.000000 jupysql-0.7.0/src/jupysql.egg-info/not-zip-safe
--rw-r--r--   0 eduardo    (501) staff       (20)      474 2023-04-05 15:53:32.000000 jupysql-0.7.0/src/jupysql.egg-info/requires.txt
--rw-r--r--   0 eduardo    (501) staff       (20)        4 2023-04-05 15:53:32.000000 jupysql-0.7.0/src/jupysql.egg-info/top_level.txt
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-05 15:53:32.412213 jupysql-0.7.0/src/sql/
--rw-r--r--   0 eduardo    (501) staff       (20)      169 2023-04-05 15:53:29.000000 jupysql-0.7.0/src/sql/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)     9701 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/_testing.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2899 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/column_guesser.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2716 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/command.py
--rw-r--r--   0 eduardo    (501) staff       (20)    14392 2023-04-04 18:22:44.000000 jupysql-0.7.0/src/sql/connection.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-05 15:53:32.412636 jupysql-0.7.0/src/sql/ggplot/
--rw-r--r--   0 eduardo    (501) staff       (20)      248 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/ggplot/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)      446 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/ggplot/aes.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1296 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/ggplot/facet_wrap.py
-drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-05 15:53:32.413063 jupysql-0.7.0/src/sql/ggplot/geom/
--rw-r--r--   0 eduardo    (501) staff       (20)      158 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/ggplot/geom/__init__.py
--rw-r--r--   0 eduardo    (501) staff       (20)      327 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/ggplot/geom/geom.py
--rw-r--r--   0 eduardo    (501) staff       (20)      463 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/ggplot/geom/geom_boxplot.py
--rw-r--r--   0 eduardo    (501) staff       (20)     1060 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/ggplot/geom/geom_histogram.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2412 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/ggplot/ggplot.py
--rw-r--r--   0 eduardo    (501) staff       (20)     8157 2023-04-04 23:50:18.000000 jupysql-0.7.0/src/sql/inspect.py
--rw-r--r--   0 eduardo    (501) staff       (20)    14744 2023-04-04 18:22:44.000000 jupysql-0.7.0/src/sql/magic.py
--rw-r--r--   0 eduardo    (501) staff       (20)     7427 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/magic_cmd.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2516 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/magic_plot.py
--rw-r--r--   0 eduardo    (501) staff       (20)     2871 2023-03-30 15:02:40.000000 jupysql-0.7.0/src/sql/parse.py
--rw-r--r--   0 eduardo    (501) staff       (20)    16590 2023-04-05 15:27:57.000000 jupysql-0.7.0/src/sql/plot.py
--rw-r--r--   0 eduardo    (501) staff       (20)    15683 2023-04-05 15:27:57.000000 jupysql-0.7.0/src/sql/run.py
--rw-r--r--   0 eduardo    (501) staff       (20)     4892 2023-04-04 18:22:44.000000 jupysql-0.7.0/src/sql/store.py
--rw-r--r--   0 eduardo    (501) staff       (20)      326 2023-03-03 23:16:57.000000 jupysql-0.7.0/src/sql/telemetry.py
--rw-r--r--   0 eduardo    (501) staff       (20)     4913 2023-04-05 15:27:57.000000 jupysql-0.7.0/src/sql/util.py
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-19 17:09:32.527426 jupysql-0.7.1/
+-rw-r--r--   0 eduardo    (501) staff       (20)    11820 2023-03-30 15:02:40.000000 jupysql-0.7.1/LICENSE
+-rw-r--r--   0 eduardo    (501) staff       (20)       52 2022-12-22 14:07:08.000000 jupysql-0.7.1/MANIFEST.in
+-rw-r--r--   0 eduardo    (501) staff       (20)     3017 2023-04-19 17:09:32.527475 jupysql-0.7.1/PKG-INFO
+-rw-r--r--   0 eduardo    (501) staff       (20)     2354 2023-04-13 14:31:32.000000 jupysql-0.7.1/README.md
+-rw-r--r--   0 eduardo    (501) staff       (20)      647 2023-04-12 23:36:02.000000 jupysql-0.7.1/pyproject.toml
+-rw-r--r--   0 eduardo    (501) staff       (20)      120 2023-04-19 17:09:32.527664 jupysql-0.7.1/setup.cfg
+-rw-r--r--   0 eduardo    (501) staff       (20)     2138 2023-04-19 17:04:46.000000 jupysql-0.7.1/setup.py
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-19 17:09:32.523170 jupysql-0.7.1/src/
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-19 17:09:32.524643 jupysql-0.7.1/src/jupysql.egg-info/
+-rw-r--r--   0 eduardo    (501) staff       (20)     3017 2023-04-19 17:09:32.000000 jupysql-0.7.1/src/jupysql.egg-info/PKG-INFO
+-rw-r--r--   0 eduardo    (501) staff       (20)      796 2023-04-19 17:09:32.000000 jupysql-0.7.1/src/jupysql.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardo    (501) staff       (20)        1 2023-04-19 17:09:32.000000 jupysql-0.7.1/src/jupysql.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardo    (501) staff       (20)        1 2022-12-22 14:07:34.000000 jupysql-0.7.1/src/jupysql.egg-info/not-zip-safe
+-rw-r--r--   0 eduardo    (501) staff       (20)      491 2023-04-19 17:09:32.000000 jupysql-0.7.1/src/jupysql.egg-info/requires.txt
+-rw-r--r--   0 eduardo    (501) staff       (20)        4 2023-04-19 17:09:32.000000 jupysql-0.7.1/src/jupysql.egg-info/top_level.txt
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-19 17:09:32.526406 jupysql-0.7.1/src/sql/
+-rw-r--r--   0 eduardo    (501) staff       (20)      169 2023-04-19 17:09:29.000000 jupysql-0.7.1/src/sql/__init__.py
+-rw-r--r--   0 eduardo    (501) staff       (20)    10319 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/_testing.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     2899 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/column_guesser.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     2716 2023-04-12 23:36:02.000000 jupysql-0.7.1/src/sql/command.py
+-rw-r--r--   0 eduardo    (501) staff       (20)    14312 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/connection.py
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-19 17:09:32.526866 jupysql-0.7.1/src/sql/ggplot/
+-rw-r--r--   0 eduardo    (501) staff       (20)      248 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/__init__.py
+-rw-r--r--   0 eduardo    (501) staff       (20)      446 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/aes.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     1331 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/ggplot/facet_wrap.py
+drwxr-xr-x   0 eduardo    (501) staff       (20)        0 2023-04-19 17:09:32.527320 jupysql-0.7.1/src/sql/ggplot/geom/
+-rw-r--r--   0 eduardo    (501) staff       (20)      158 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/geom/__init__.py
+-rw-r--r--   0 eduardo    (501) staff       (20)      327 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/geom/geom.py
+-rw-r--r--   0 eduardo    (501) staff       (20)      463 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/geom/geom_boxplot.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     1060 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/geom/geom_histogram.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     2412 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/ggplot/ggplot.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     9231 2023-04-13 01:27:43.000000 jupysql-0.7.1/src/sql/inspect.py
+-rw-r--r--   0 eduardo    (501) staff       (20)    14701 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/magic.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     8803 2023-04-19 17:04:46.000000 jupysql-0.7.1/src/sql/magic_cmd.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     2516 2023-03-30 15:02:40.000000 jupysql-0.7.1/src/sql/magic_plot.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     2923 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/parse.py
+-rw-r--r--   0 eduardo    (501) staff       (20)    16880 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/plot.py
+-rw-r--r--   0 eduardo    (501) staff       (20)    15767 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/run.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     4868 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/store.py
+-rw-r--r--   0 eduardo    (501) staff       (20)      326 2023-03-03 23:16:57.000000 jupysql-0.7.1/src/sql/telemetry.py
+-rw-r--r--   0 eduardo    (501) staff       (20)     5096 2023-04-12 23:53:59.000000 jupysql-0.7.1/src/sql/util.py
```

### Comparing `jupysql-0.7.0/LICENSE` & `jupysql-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.0/PKG-INFO` & `jupysql-0.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.0
+Version: 0.7.1
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
@@ -58,14 +58,20 @@
 
 ## Installation
 
 ```
 pip install jupysql
 ```
 
+or:
+
+```
+conda install jupysql -c conda-forge
+```
+
 ## Documentation
 
 [Click here to see the documentation.](https://jupysql.ploomber.io)
 
 
 ## Credits
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.0 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.1 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
@@ -21,14 +21,14 @@
 Run SQL in Jupyter/IPython via a `%sql` and `%%sql` magics.
                                  [Get_Started]
 ## Features - [Pandas integration](https://jupysql.ploomber.io/en/latest/
 integrations/pandas.html) - [SQL composition (no more hard-to-debug CTEs!)]
 (https://jupysql.ploomber.io/en/latest/compose.html) - [Plot massive datasets
 without blowing up memory](https://jupysql.ploomber.io/en/latest/plot.html) -
 [DuckDB integration](https://jupysql.ploomber.io/en/latest/integrations/
-duckdb.html) ## Installation ``` pip install jupysql ``` ## Documentation
-[Click here to see the documentation.](https://jupysql.ploomber.io) ## Credits
-This project is a fork of [ipython-sql](https://github.com/catherinedevlin/
-ipython-sql); the objective is to turn this project into a full-featured SQL
-client for Jupyter. We're looking for feedback and taking feature requests, so
-please [join our community](https://ploomber.io/community) and enter the
-#jupysql channel.
+duckdb.html) ## Installation ``` pip install jupysql ``` or: ``` conda install
+jupysql -c conda-forge ``` ## Documentation [Click here to see the
+documentation.](https://jupysql.ploomber.io) ## Credits This project is a fork
+of [ipython-sql](https://github.com/catherinedevlin/ipython-sql); the objective
+is to turn this project into a full-featured SQL client for Jupyter. We're
+looking for feedback and taking feature requests, so please [join our
+community](https://ploomber.io/community) and enter the #jupysql channel.
```

### Comparing `jupysql-0.7.0/README.md` & `jupysql-0.7.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,20 @@
 
 ## Installation
 
 ```
 pip install jupysql
 ```
 
+or:
+
+```
+conda install jupysql -c conda-forge
+```
+
 ## Documentation
 
 [Click here to see the documentation.](https://jupysql.ploomber.io)
 
 
 ## Credits
```

#### html2text {}

```diff
@@ -12,14 +12,14 @@
 Run SQL in Jupyter/IPython via a `%sql` and `%%sql` magics.
                                  [Get_Started]
 ## Features - [Pandas integration](https://jupysql.ploomber.io/en/latest/
 integrations/pandas.html) - [SQL composition (no more hard-to-debug CTEs!)]
 (https://jupysql.ploomber.io/en/latest/compose.html) - [Plot massive datasets
 without blowing up memory](https://jupysql.ploomber.io/en/latest/plot.html) -
 [DuckDB integration](https://jupysql.ploomber.io/en/latest/integrations/
-duckdb.html) ## Installation ``` pip install jupysql ``` ## Documentation
-[Click here to see the documentation.](https://jupysql.ploomber.io) ## Credits
-This project is a fork of [ipython-sql](https://github.com/catherinedevlin/
-ipython-sql); the objective is to turn this project into a full-featured SQL
-client for Jupyter. We're looking for feedback and taking feature requests, so
-please [join our community](https://ploomber.io/community) and enter the
-#jupysql channel.
+duckdb.html) ## Installation ``` pip install jupysql ``` or: ``` conda install
+jupysql -c conda-forge ``` ## Documentation [Click here to see the
+documentation.](https://jupysql.ploomber.io) ## Credits This project is a fork
+of [ipython-sql](https://github.com/catherinedevlin/ipython-sql); the objective
+is to turn this project into a full-featured SQL client for Jupyter. We're
+looking for feedback and taking feature requests, so please [join our
+community](https://ploomber.io/community) and enter the #jupysql channel.
```

### Comparing `jupysql-0.7.0/pyproject.toml` & `jupysql-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.0/setup.py` & `jupysql-0.7.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,29 +14,29 @@
     VERSION = str(
         ast.literal_eval(_version_re.search(f.read().decode("utf-8")).group(1))
     )
 
 install_requires = [
     "prettytable",
     "ipython>=1.0",
-    "sqlalchemy<2",
+    "sqlalchemy",
     "sqlparse",
     "ipython-genutils>=0.1.0",
     "sqlglot",
     "jinja2",
     "sqlglot>=11.3.7",
     "ploomber-core>=0.2.7",
     'importlib-metadata;python_version<"3.8"',
 ]
 
 DEV = [
     "flake8",
     "pytest",
     "pandas",
-    "polars==0.16.14",  # 03/24/23 this breaks our CI
+    "polars==0.17.2",  # 04/18/23 this breaks our CI
     "invoke",
     "pkgmt",
     "twine",
     # tests
     "duckdb",
     "duckdb-engine",
     "pyodbc",
@@ -51,14 +51,15 @@
 INTEGRATION = [
     "dockerctx",
     "pyarrow",
     "psycopg2-binary",
     "pymysql",
     "pgspecial==2.0.1",
     "pyodbc",
+    "snowflake-sqlalchemy",
 ]
 
 setup(
     name="jupysql",
     version=VERSION,
     description="Better SQL in Jupyter",
     long_description=README,
```

### Comparing `jupysql-0.7.0/src/jupysql.egg-info/PKG-INFO` & `jupysql-0.7.1/src/jupysql.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.0
+Version: 0.7.1
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
@@ -58,14 +58,20 @@
 
 ## Installation
 
 ```
 pip install jupysql
 ```
 
+or:
+
+```
+conda install jupysql -c conda-forge
+```
+
 ## Documentation
 
 [Click here to see the documentation.](https://jupysql.ploomber.io)
 
 
 ## Credits
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.0 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.1 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
@@ -21,14 +21,14 @@
 Run SQL in Jupyter/IPython via a `%sql` and `%%sql` magics.
                                  [Get_Started]
 ## Features - [Pandas integration](https://jupysql.ploomber.io/en/latest/
 integrations/pandas.html) - [SQL composition (no more hard-to-debug CTEs!)]
 (https://jupysql.ploomber.io/en/latest/compose.html) - [Plot massive datasets
 without blowing up memory](https://jupysql.ploomber.io/en/latest/plot.html) -
 [DuckDB integration](https://jupysql.ploomber.io/en/latest/integrations/
-duckdb.html) ## Installation ``` pip install jupysql ``` ## Documentation
-[Click here to see the documentation.](https://jupysql.ploomber.io) ## Credits
-This project is a fork of [ipython-sql](https://github.com/catherinedevlin/
-ipython-sql); the objective is to turn this project into a full-featured SQL
-client for Jupyter. We're looking for feedback and taking feature requests, so
-please [join our community](https://ploomber.io/community) and enter the
-#jupysql channel.
+duckdb.html) ## Installation ``` pip install jupysql ``` or: ``` conda install
+jupysql -c conda-forge ``` ## Documentation [Click here to see the
+documentation.](https://jupysql.ploomber.io) ## Credits This project is a fork
+of [ipython-sql](https://github.com/catherinedevlin/ipython-sql); the objective
+is to turn this project into a full-featured SQL client for Jupyter. We're
+looking for feedback and taking feature requests, so please [join our
+community](https://ploomber.io/community) and enter the #jupysql channel.
```

### Comparing `jupysql-0.7.0/src/jupysql.egg-info/SOURCES.txt` & `jupysql-0.7.1/src/jupysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.0/src/sql/_testing.py` & `jupysql-0.7.1/src/sql/_testing.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from dockerctx import new_container
 from contextlib import contextmanager
 import sys
 import time
 import docker
 from docker import errors
 from sqlalchemy.engine import URL
+import os
+
 
 TMP_DIR = "tmp"
 
 
 class DatabaseConfigHelper:
     @staticmethod
     def get_database_config(database):
@@ -106,14 +108,29 @@
         "docker_ct": {
             "name": "MSSQL",
             "image": "mcr.microsoft.com/azure-sql-edge",
             "ports": {1433: 1433},
         },
         "alias": "MSSQLTest",
     },
+    "Snowflake": {
+        "drivername": "snowflake",
+        "username": os.getenv("SF_USERNAME"),
+        "password": os.getenv("SF_PASSWORD"),
+        # database/schema
+        "database": os.getenv("SF_DATABASE"),
+        "host": "lpb17716.us-east-1",
+        "port": None,
+        "alias": "snowflakeTest",
+        "docker_ct": None,
+        "query": {
+            "warehouse": "COMPUTE_WH",
+            "role": "SYSADMIN",
+        },
+    },
 }
 
 
 # SQLAlchmey URL: https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls
 def _get_database_url(database):
     return URL.create(
         drivername=databaseConfig[database]["drivername"],
@@ -128,39 +145,44 @@
 
 client = docker.from_env()
 
 
 def database_ready(
     database,
     timeout=20,
-    poll_freq=0.2,
+    poll_freq=0.5,
 ):
-    """Wait until a postgres instance is ready to receive connections.
+    """Wait until the container is ready to receive connections.
 
-    .. note::
-
-        This requires psycopg2 to be installed.
 
     :type host: str
     :type port: int
     :type timeout: float
     :type poll_freq: float
     """
     import sqlalchemy
 
+    errors = []
+
     t0 = time.time()
     while time.time() - t0 < timeout:
         try:
             eng = sqlalchemy.create_engine(_get_database_url(database)).connect()
             eng.close()
             return True
-        except Exception:
-            pass
+        except Exception as e:
+            errors.append(str(e))
+
         time.sleep(poll_freq)
 
+    # print all the errors so we know what's goin on since failing to connect might be
+    # to some misconfiguration error
+    errors_ = "\n".join(errors)
+    print(f"ERRORS: {errors_}")
+
     return False
 
 
 @contextmanager
 def postgres(is_bypass_init=False):
     if is_bypass_init:
         yield None
```

### Comparing `jupysql-0.7.0/src/sql/column_guesser.py` & `jupysql-0.7.1/src/sql/column_guesser.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.0/src/sql/command.py` & `jupysql-0.7.1/src/sql/command.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.0/src/sql/connection.py` & `jupysql-0.7.1/src/sql/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -345,107 +345,103 @@
             cls.connections.pop(descriptor)
         else:
             cls.connections.pop(
                 str(conn.metadata.bind.url) if IS_SQLALCHEMY_ONE else str(conn.url)
             )
             conn.session.close()
 
-    @classmethod
-    def _get_curr_sqlalchemy_connection_info(cls):
+    def _get_curr_sqlalchemy_connection_info(self):
         """Get the dialect, driver, and database server version info of current
         connected dialect
 
         Returns
         -------
         dict
             The dictionary which contains the SQLAlchemy-based dialect
             information, or None if there is no current connection.
         """
-        if not cls.current:
+
+        if not self.session:
             return None
+        engine = self.metadata.bind if IS_SQLALCHEMY_ONE else self.session
 
-        engine = cls.current.metadata.bind if IS_SQLALCHEMY_ONE else cls.current
         return {
             "dialect": getattr(engine.dialect, "name", None),
             "driver": getattr(engine.dialect, "driver", None),
             "server_version_info": getattr(engine.dialect, "server_version_info", None),
         }
 
-    @classmethod
-    def _get_curr_sqlglot_dialect(cls):
+    def _get_curr_sqlglot_dialect(self):
         """Get the dialect name in sqlglot package scope
 
         Returns
         -------
         str
             Available dialect in sqlglot package, see more:
             https://github.com/tobymao/sqlglot/blob/main/sqlglot/dialects/dialect.py
         """
-        connection_info = cls._get_curr_sqlalchemy_connection_info()
+        connection_info = self._get_curr_sqlalchemy_connection_info()
         if not connection_info:
             return None
 
         return DIALECT_NAME_SQLALCHEMY_TO_SQLGLOT_MAPPING.get(
             connection_info["dialect"], connection_info["dialect"]
         )
 
-    @classmethod
-    def is_use_backtick_template(cls):
+    def is_use_backtick_template(self):
         """Get if the dialect support backtick (`) syntax as identifier
 
         Returns
         -------
         bool
             Indicate if the dialect can use backtick identifier in the SQL clause
         """
-        cur_dialect = cls._get_curr_sqlglot_dialect()
+        cur_dialect = self._get_curr_sqlglot_dialect()
         if not cur_dialect:
             return False
         try:
             return (
                 "`" in sqlglot.Dialect.get_or_raise(cur_dialect).Tokenizer.IDENTIFIERS
             )
         except (ValueError, AttributeError, TypeError):
             return False
 
-    @classmethod
-    def _transpile_query(cls, query):
-        """Translate the given SQL clause that's compatible to current connected
-        dialect by sqlglot
-
-        Parameters
-        ----------
-        query : str
-            Original SQL clause
-
-        Returns
-        -------
-        str
-            SQL clause that's compatible to current connected dialect
-        """
-        write_dialect = cls._get_curr_sqlglot_dialect()
-        try:
-            query = sqlglot.parse_one(query).sql(dialect=write_dialect)
-        finally:
-            return query
-
-    @classmethod
-    def get_curr_identifiers(cls) -> list:
+    def get_curr_identifiers(self) -> list:
         """
         Returns list of identifiers for current connection
 
         Default identifiers are : ["", '"']
         """
         identifiers = ["", '"']
         try:
-            connection_info = cls._get_curr_sqlalchemy_connection_info()
+            connection_info = self._get_curr_sqlalchemy_connection_info()
             if connection_info:
                 cur_dialect = connection_info["dialect"]
                 identifiers_ = sqlglot.Dialect.get_or_raise(
                     cur_dialect
                 ).Tokenizer.IDENTIFIERS
 
                 identifiers = [*set(identifiers + identifiers_)]
         except ValueError:
             pass
 
         return identifiers
+
+    def _transpile_query(self, query):
+        """Translate the given SQL clause that's compatible to current connected
+        dialect by sqlglot
+
+        Parameters
+        ----------
+        query : str
+            Original SQL clause
+
+        Returns
+        -------
+        str
+            SQL clause that's compatible to current connected dialect
+        """
+        write_dialect = self._get_curr_sqlglot_dialect()
+        try:
+            query = sqlglot.parse_one(query).sql(dialect=write_dialect)
+        finally:
+            return query
```

### Comparing `jupysql-0.7.0/src/sql/ggplot/facet_wrap.py` & `jupysql-0.7.1/src/sql/ggplot/facet_wrap.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from jinja2 import Template
 import math
 import sql.connection
 from sql.store import store
 from sql.telemetry import telemetry
+import sqlalchemy
 
 
 def _run_query(query, with_=None, conn=None):
     if not conn:
         conn = sql.connection.Connection.current.session
 
     if with_:
         query = str(store.render(query, with_=with_))
 
-    return conn.execute(query).fetchall()
+    return conn.execute(sqlalchemy.text(query)).fetchall()
 
 
 class facet:
     def __init__():
         pass
 
     def get_facet_values(self, table, column, with_):
```

### Comparing `jupysql-0.7.0/src/sql/ggplot/geom/geom_histogram.py` & `jupysql-0.7.1/src/sql/ggplot/geom/geom_histogram.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.0/src/sql/ggplot/ggplot.py` & `jupysql-0.7.1/src/sql/ggplot/ggplot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.0/src/sql/magic.py` & `jupysql-0.7.1/src/sql/magic.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,17 +337,15 @@
         conn = sql.connection.Connection.set(
             connect_arg,
             displaycon=self.displaycon,
             connect_args=args.connection_arguments,
             creator=args.creator,
             alias=args.alias,
         )
-        payload[
-            "connection_info"
-        ] = sql.connection.Connection._get_curr_sqlalchemy_connection_info()
+        payload["connection_info"] = conn._get_curr_sqlalchemy_connection_info()
         if args.persist:
             return self._persist_dataframe(
                 command.sql, conn, user_ns, append=False, index=not args.no_index
             )
 
         if args.append:
             return self._persist_dataframe(
```

### Comparing `jupysql-0.7.0/src/sql/magic_cmd.py` & `jupysql-0.7.1/src/sql/magic_cmd.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from IPython.utils.process import arg_split
 from IPython.core.magic import Magics, line_magic, magics_class
 from IPython.core.magic_arguments import argument, magic_arguments
 from IPython.core.error import UsageError
 from sqlglot import select, condition
 from sqlalchemy import text
 
+from prettytable import PrettyTable
+
 try:
     from traitlets.config.configurable import Configurable
 except ImportError:
     from IPython.config.configurable import Configurable
 
 import sql.connection
 from sql import inspect
@@ -131,33 +133,54 @@
                 "-nn",
                 "--no-nulls",
                 help="Returns rows in specified column that are not null.",
                 action="store_true",
             )
 
             args = parser.parse_args(others)
+
+            COMPARATOR_ARGS = [
+                args.greater,
+                args.greater_or_equal,
+                args.less_than,
+                args.less_than_or_equal,
+            ]
+
+            if args.table and not any(COMPARATOR_ARGS):
+                raise UsageError("Please use a valid comparator.")
+
+            if args.table and any(COMPARATOR_ARGS) and not args.column:
+                raise UsageError("Please pass a column to test.")
+
             if args.greater and args.greater_or_equal:
                 return ValueError(
                     "You cannot use both greater and greater "
                     "than or equal to arguments at the same time."
                 )
             elif args.less_than and args.less_than_or_equal:
                 return ValueError(
                     "You cannot use both less and less than "
                     "or equal to arguments at the same time."
                 )
 
             conn = sql.connection.Connection.current.session
             result_dict = run_each_individually(args, conn)
 
-            if len(result_dict.keys()):
-                print(
-                    "Test failed. Returned are samples of the failures from your data:"
+            if any(len(rows) > 1 for rows in list(result_dict.values())):
+                for comparator, rows in result_dict.items():
+                    if len(rows) > 1:
+                        print(f"\n{comparator}:\n")
+                        _pretty = PrettyTable()
+                        _pretty.field_names = rows[0]
+                        for row in rows[1:]:
+                            _pretty.add_row(row)
+                        print(_pretty)
+                raise UsageError(
+                    "The above values do not not match your test requirements."
                 )
-                return result_dict
             else:
                 return True
 
         elif cmd_name == "profile":
             parser = CmdParser()
             parser.add_argument(
                 "-t", "--table", type=str, help="Table name", required=True
@@ -178,50 +201,70 @@
             if args.output:
                 with open(args.output, "w") as f:
                     f.write(report._repr_html_())
 
             return report
 
 
+def return_test_results(args, conn, query):
+    try:
+        columns = []
+        column_data = conn.execute(text(query)).cursor.description
+        res = conn.execute(text(query)).fetchall()
+        for column in column_data:
+            columns.append(column[0])
+        res = [columns, *res]
+        return res
+    except Exception as e:
+        if "column" in str(e):
+            raise UsageError(f"Referenced column '{args.column}' not found!")
+
+
 def run_each_individually(args, conn):
     base_query = select("*").from_(args.table)
+
     storage = {}
 
     if args.greater:
-        where = condition(args.column + ">" + args.greater)
+        where = condition(args.column + "<=" + args.greater)
         current_query = base_query.where(where).sql()
 
-        res = conn.execute(text(current_query)).fetchone()
+        res = return_test_results(args, conn, query=current_query)
 
         if res is not None:
             storage["greater"] = res
     if args.greater_or_equal:
-        where = condition(args.column + ">=" + args.greater_or_equal)
+        where = condition(args.column + "<" + args.greater_or_equal)
 
         current_query = base_query.where(where).sql()
 
-        res = conn.execute(text(current_query)).fetchone()
+        res = return_test_results(args, conn, query=current_query)
+
         if res is not None:
             storage["greater_or_equal"] = res
+
     if args.less_than_or_equal:
-        where = condition(args.column + "<=" + args.less_than_or_equal)
+        where = condition(args.column + ">" + args.less_than_or_equal)
         current_query = base_query.where(where).sql()
 
-        res = conn.execute(text(current_query)).fetchone()
+        res = return_test_results(args, conn, query=current_query)
+
         if res is not None:
             storage["less_than_or_equal"] = res
     if args.less_than:
-        where = condition(args.column + "<" + args.less_than)
+        where = condition(args.column + ">=" + args.less_than)
         current_query = base_query.where(where).sql()
 
-        res = conn.execute(text(current_query)).fetchone()
+        res = return_test_results(args, conn, query=current_query)
+
         if res is not None:
             storage["less_than"] = res
     if args.no_nulls:
         where = condition("{} is NULL".format(args.column))
         current_query = base_query.where(where).sql()
 
-        res = conn.execute(text(current_query)).fetchone()
+        res = return_test_results(args, conn, query=current_query)
+
         if res is not None:
             storage["null"] = res
 
     return storage
```

### Comparing `jupysql-0.7.0/src/sql/magic_plot.py` & `jupysql-0.7.1/src/sql/magic_plot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.0/src/sql/parse.py` & `jupysql-0.7.1/src/sql/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 from IPython.core.magic_arguments import parse_argstring
 
 
 def connection_from_dsn_section(section, config):
     parser = CP.ConfigParser()
     parser.read(config.dsn_filename)
     cfg_dict = dict(parser.items(section))
-    return str(URL(**cfg_dict))
+    return str(URL.create(**cfg_dict).render_as_string(hide_password=False))
 
 
 def _connection_string(s, config):
     s = expandvars(s)  # for environment variables
     if "@" in s or "://" in s:
         return s
     if s.startswith("[") and s.endswith("]"):
         section = s.lstrip("[").rstrip("]")
         parser = CP.ConfigParser()
         parser.read(config.dsn_filename)
         cfg_dict = dict(parser.items(section))
-        return str(URL(**cfg_dict))
+        return str(URL.create(**cfg_dict))
     return ""
 
 
 def parse(cell, config):
     """Extract connection info and result variable from SQL
 
     Please don't add any more syntax requiring
```

### Comparing `jupysql-0.7.0/src/sql/plot.py` & `jupysql-0.7.1/src/sql/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 
 from sql.store import store
 import sql.connection
 from sql.telemetry import telemetry
 import warnings
 
 
-def _summary_stats(con, table, column, with_=None):
+def _summary_stats(conn, table, column, with_=None):
+    if not conn:
+        conn = sql.connection.Connection.current
     """Compute percentiles and mean for boxplot"""
     template = Template(
         """
 SELECT
 percentile_disc(0.25) WITHIN GROUP (ORDER BY "{{column}}") AS q1,
 percentile_disc(0.50) WITHIN GROUP (ORDER BY "{{column}}") AS med,
 percentile_disc(0.75) WITHIN GROUP (ORDER BY "{{column}}") AS q3,
@@ -38,20 +40,22 @@
 """
     )
     query = template.render(table=table, column=column)
 
     if with_:
         query = str(store.render(query, with_=with_))
 
-    values = con.execute(sqlalchemy.sql.text(query)).fetchone()
+    values = conn.session.execute(sqlalchemy.sql.text(query)).fetchone()
     keys = ["q1", "med", "q3", "mean", "N"]
     return {k: float(v) for k, v in zip(keys, values)}
 
 
-def _whishi(con, table, column, hival, with_=None):
+def _whishi(conn, table, column, hival, with_=None):
+    if not conn:
+        conn = sql.connection.Connection.current
     template = Template(
         """
 SELECT COUNT(*), MAX("{{column}}")
 FROM (
     SELECT "{{column}}"
     FROM "{{table}}"
     WHERE "{{column}}" <= {{hival}}
@@ -59,21 +63,23 @@
 """
     )
 
     query = template.render(table=table, column=column, hival=hival)
 
     if with_:
         query = str(store.render(query, with_=with_))
-    query = sql.connection.Connection._transpile_query(query)
-    values = con.execute(sqlalchemy.sql.text(query)).fetchone()
+    query = conn._transpile_query(query)
+    values = conn.session.execute(sqlalchemy.sql.text(query)).fetchone()
     keys = ["N", "wiskhi_max"]
     return {k: float(v) for k, v in zip(keys, values)}
 
 
-def _whislo(con, table, column, loval, with_=None):
+def _whislo(conn, table, column, loval, with_=None):
+    if not conn:
+        conn = sql.connection.Connection.current
     template = Template(
         """
 SELECT COUNT(*), MIN("{{column}}")
 FROM (
     SELECT "{{column}}"
     FROM "{{table}}"
     WHERE "{{column}}" >= {{loval}}
@@ -81,70 +87,76 @@
 """
     )
 
     query = template.render(table=table, column=column, loval=loval)
 
     if with_:
         query = str(store.render(query, with_=with_))
-    query = sql.connection.Connection._transpile_query(query)
-    values = con.execute(sqlalchemy.sql.text(query)).fetchone()
+    query = conn._transpile_query(query)
+    values = conn.session.execute(sqlalchemy.sql.text(query)).fetchone()
     keys = ["N", "wisklo_min"]
     return {k: float(v) for k, v in zip(keys, values)}
 
 
-def _percentile(con, table, column, pct, with_=None):
+def _percentile(conn, table, column, pct, with_=None):
+    if not conn:
+        conn = sql.connection.Connection.current.session
     template = Template(
         """
 SELECT
 percentile_disc({{pct}}) WITHIN GROUP (ORDER BY "{{column}}") AS pct,
 FROM "{{table}}"
 """
     )
     query = template.render(table=table, column=column, pct=pct)
 
     if with_:
         query = str(store.render(query, with_=with_))
-    query = sql.connection.Connection._transpile_query(query)
-    values = con.execute(sqlalchemy.sql.text(query)).fetchone()[0]
+    query = conn._transpile_query(query)
+    values = conn.session.execute(sqlalchemy.sql.text(query)).fetchone()[0]
     return values
 
 
-def _between(con, table, column, whislo, whishi, with_=None):
+def _between(conn, table, column, whislo, whishi, with_=None):
     template = Template(
         """
 SELECT "{{column}}"
 FROM "{{table}}"
 WHERE "{{column}}" < {{whislo}}
 OR  "{{column}}" > {{whishi}}
 """
     )
     query = template.render(table=table, column=column, whislo=whislo, whishi=whishi)
 
     if with_:
         query = str(store.render(query, with_=with_))
-    query = sql.connection.Connection._transpile_query(query)
-    results = [float(n[0]) for n in con.execute(sqlalchemy.sql.text(query)).fetchall()]
+    query = conn._transpile_query(query)
+    results = [
+        float(n[0]) for n in conn.session.execute(sqlalchemy.sql.text(query)).fetchall()
+    ]
     return results
 
 
 # https://github.com/matplotlib/matplotlib/blob/b5ac96a8980fdb9e59c9fb649e0714d776e26701/lib/matplotlib/cbook/__init__.py
 @modify_exceptions
-def _boxplot_stats(con, table, column, whis=1.5, autorange=False, with_=None):
+def _boxplot_stats(conn, table, column, whis=1.5, autorange=False, with_=None):
+    if not conn:
+        conn = sql.connection.Connection.current
     """Compute statistics required to create a boxplot"""
 
     def _compute_conf_interval(N, med, iqr):
         notch_min = med - 1.57 * iqr / np.sqrt(N)
         notch_max = med + 1.57 * iqr / np.sqrt(N)
 
         return notch_min, notch_max
 
     stats = dict()
 
     # arithmetic mean
-    s_stats = _summary_stats(con, table, column, with_=with_)
+    s_stats = _summary_stats(conn, table, column, with_=with_)
 
     stats["mean"] = s_stats["mean"]
     q1, med, q3 = s_stats["q1"], s_stats["med"], s_stats["q3"]
     N = s_stats["N"]
 
     # interquartile range
     stats["iqr"] = q3 - q1
@@ -153,41 +165,41 @@
         whis = (0, 100)
 
     # conf. interval around median
     stats["cilo"], stats["cihi"] = _compute_conf_interval(N, med, stats["iqr"])
 
     # lowest/highest non-outliers
     if np.iterable(whis) and not isinstance(whis, str):
-        loval, hival = _percentile(con, table, column, whis, with_=with_)
+        loval, hival = _percentile(conn, table, column, whis, with_=with_)
 
     elif np.isreal(whis):
         loval = q1 - whis * stats["iqr"]
         hival = q3 + whis * stats["iqr"]
     else:
         raise ValueError("whis must be a float or list of percentiles")
 
     # get high extreme
-    wiskhi_d = _whishi(con, table, column, hival, with_=with_)
+    wiskhi_d = _whishi(conn, table, column, hival, with_=with_)
 
     if wiskhi_d["N"] == 0 or wiskhi_d["wiskhi_max"] < q3:
         stats["whishi"] = q3
     else:
         stats["whishi"] = wiskhi_d["wiskhi_max"]
 
     # get low extreme
-    wisklo_d = _whislo(con, table, column, loval, with_=with_)
+    wisklo_d = _whislo(conn, table, column, loval, with_=with_)
 
     if wisklo_d["N"] == 0 or wisklo_d["wisklo_min"] > q1:
         stats["whislo"] = q1
     else:
         stats["whislo"] = wisklo_d["wisklo_min"]
 
     # compute a single array of outliers
     stats["fliers"] = np.array(
-        _between(con, table, column, stats["whislo"], stats["whishi"], with_=with_)
+        _between(conn, table, column, stats["whislo"], stats["whishi"], with_=with_)
     )
 
     # add in the remaining stats
     stats["q1"], stats["med"], stats["q3"] = q1, med, q3
 
     bxpstats = {k: v for k, v in stats.items()}
 
@@ -241,19 +253,17 @@
     .. plot:: ../examples/plot_boxplot_horizontal.py
 
     **Plot multiple columns from the same table:**
 
     .. plot:: ../examples/plot_boxplot_many.py
     """
     if not conn:
-        conn = sql.connection.Connection.current.session
+        conn = sql.connection.Connection.current
 
-    payload[
-        "connection_info"
-    ] = sql.connection.Connection._get_curr_sqlalchemy_connection_info()
+    payload["connection_info"] = conn._get_curr_sqlalchemy_connection_info()
 
     ax = plt.gca()
     vert = orient == "v"
 
     set_ticklabels = ax.set_xticklabels if vert else ax.set_yticklabels
     set_label = ax.set_ylabel if vert else ax.set_xlabel
 
@@ -269,31 +279,32 @@
         ax.set_title(f"Boxplot from {table!r}")
         set_ticklabels(column)
 
     return ax
 
 
 def _min_max(con, table, column, with_=None, use_backticks=False):
+    if not con:
+        con = sql.connection.Connection.current
     template_ = """
 SELECT
     MIN("{{column}}"),
     MAX("{{column}}")
 FROM "{{table}}"
 """
-
     if use_backticks:
         template_ = template_.replace('"', "`")
 
     template = Template(template_)
     query = template.render(table=table, column=column)
 
     if with_:
         query = str(store.render(query, with_=with_))
-    query = sql.connection.Connection._transpile_query(query)
-    min_, max_ = con.execute(sqlalchemy.sql.text(query)).fetchone()
+    query = con._transpile_query(query)
+    min_, max_ = con.session.execute(sqlalchemy.sql.text(query)).fetchone()
     return min_, max_
 
 
 def _are_numeric_values(*values):
     return all([isinstance(value, (int, float)) for value in values])
 
 
@@ -363,18 +374,20 @@
     --------
     .. plot:: ../examples/plot_histogram.py
 
     **Plot multiple columns from the same table**:
 
     .. plot:: ../examples/plot_histogram_many.py
     """
+    if not conn:
+        conn = sql.connection.Connection.current
+
+    print("Current conn: ", conn)
     ax = ax or plt.gca()
-    payload[
-        "connection_info"
-    ] = sql.connection.Connection._get_curr_sqlalchemy_connection_info()
+    payload["connection_info"] = conn._get_curr_sqlalchemy_connection_info()
     if category:
         if isinstance(column, list):
             if len(column) > 1:
                 raise ValueError(
                     f"""Columns given : {column}.
                     When using a stacked histogram,
                     please ensure that you specify only one column."""
@@ -481,19 +494,16 @@
     return ax
 
 
 @modify_exceptions
 def _histogram(table, column, bins, with_=None, conn=None, facet=None):
     """Compute bins and heights"""
     if not conn:
-        conn = sql.connection.Connection.current.session
-        use_backticks = sql.connection.Connection.is_use_backtick_template()
-    else:
-        # TODO: fix
-        use_backticks = False
+        conn = sql.connection.Connection.current
+    use_backticks = conn.is_use_backtick_template()
 
     # FIXME: we're computing all the with elements twice
     min_, max_ = _min_max(conn, table, column, with_=with_, use_backticks=use_backticks)
 
     filter_query = f"WHERE {facet['key']} == '{facet['value']}'" if facet else ""
 
     bin_size = None
@@ -541,16 +551,16 @@
         template = Template(template_)
 
         query = template.render(table=table, column=column, filter_query=filter_query)
 
     if with_:
         query = str(store.render(query, with_=with_))
 
-    query = sql.connection.Connection._transpile_query(query)
-    data = conn.execute(sqlalchemy.sql.text(query)).fetchall()
+    query = conn._transpile_query(query)
+    data = conn.session.execute(sqlalchemy.sql.text(query)).fetchall()
     bin_, height = zip(*data)
 
     if bin_[0] is None:
         raise ValueError("Data contains NULLs")
 
     return bin_, height, bin_size
 
@@ -564,15 +574,15 @@
     bin_size,
     with_=None,
     conn=None,
     facet=None,
 ):
     """Compute the corresponding heights of each bin based on the category"""
     if not conn:
-        conn = sql.connection.Connection.current.session
+        conn = sql.connection.Connection.current
 
     cases = []
     for bin in bins:
         case = f'SUM(CASE WHEN floor = {bin} THEN count ELSE 0 END) AS "{bin}",'
         cases.append(case)
 
     cases = " ".join(cases)
@@ -601,11 +611,11 @@
         filter_query=filter_query,
         cases=cases,
     )
 
     if with_:
         query = str(store.render(query, with_=with_))
 
-    query = sql.connection.Connection._transpile_query(query)
-    data = conn.execute(query).fetchall()
+    query = conn._transpile_query(query)
+    data = conn.session.execute(sqlalchemy.sql.text(query)).fetchall()
 
     return data
```

### Comparing `jupysql-0.7.0/src/sql/run.py` & `jupysql-0.7.1/src/sql/run.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import sql.connection
 from .column_guesser import ColumnGuesserMixin
 
 try:
     from pgspecial.main import PGSpecial
 except ImportError:
     PGSpecial = None
+from sqlalchemy.orm import Session
 
 from sql.telemetry import telemetry
 import logging
 import warnings
 
 
 def unduplicate_field_names(field_names):
@@ -176,15 +177,15 @@
     def DataFrame(self, payload):
         "Returns a Pandas DataFrame instance built from the result set."
         import pandas as pd
 
         frame = pd.DataFrame(self, columns=(self and self.keys) or [])
         payload[
             "connection_info"
-        ] = sql.connection.Connection._get_curr_sqlalchemy_connection_info()
+        ] = sql.connection.Connection.current._get_curr_sqlalchemy_connection_info()
         return frame
 
     @telemetry.log_call("polars-data-frame")
     def PolarsDataFrame(self, **polars_dataframe_kwargs):
         "Returns a Polars DataFrame instance built from the result set."
         import polars as pl
 
@@ -386,15 +387,16 @@
             dialect not in str(conn.dialect) for dialect in _COMMIT_BLACKLIST_DIALECTS
         )
         and manual_commit
     )
 
     if _should_commit:
         try:
-            conn.session.execute("commit")
+            with Session(conn.session) as session:
+                session.commit()
         except sqlalchemy.exc.OperationalError:
             print("The database does not support the COMMIT command")
 
 
 def is_postgres_or_redshift(dialect):
     """Checks if dialect is postgres or redshift"""
     return "postgres" in str(dialect) or "redshift" in str(dialect)
```

### Comparing `jupysql-0.7.0/src/sql/store.py` & `jupysql-0.7.1/src/sql/store.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,26 +96,26 @@
                 + ", ".join(self._with_).replace("-", "_")
                 + " instead for the with argument.",
                 FutureWarning,
             )
 
     def __str__(self) -> str:
         """
-        Since some dialects don't support " (double quote) symbol, we will
-        replace to the ' (backtick) symbol if it's supported
+        We use the ' (backtick symbol) to wrap the CTE alias if the dialect supports
+        ` (backtick)
         """
         with_clause_template = Template(
-            """WITH{% for name in with_ %} "{{name}}" AS ({{saved[name]._query}})\
+            """WITH{% for name in with_ %} {{name}} AS ({{saved[name]._query}})\
 {{ "," if not loop.last }}{% endfor %}{{query}}"""
         )
         with_clause_template_backtick = Template(
             """WITH{% for name in with_ %} `{{name}}` AS ({{saved[name]._query}})\
 {{ "," if not loop.last }}{% endfor %}{{query}}"""
         )
-        is_use_backtick = sql.connection.Connection.is_use_backtick_template()
+        is_use_backtick = sql.connection.Connection.current.is_use_backtick_template()
         with_all = _get_dependencies(self._store, self._with_)
         template = (
             with_clause_template_backtick if is_use_backtick else with_clause_template
         )
         return template.render(
             query=self._query, saved=self._store._data, with_=with_all
         )
```

### Comparing `jupysql-0.7.0/src/sql/util.py` & `jupysql-0.7.1/src/sql/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,19 @@
         split_by_decimal = str(num).split(".")
         if len(split_by_decimal[0]) > 10 or len(split_by_decimal[1]) > 10:
             return True
     return False
 
 
 def is_table_exists(
-    table: str, schema: str = None, ignore_error: bool = False, with_: str = None
+    table: str,
+    schema: str = None,
+    ignore_error: bool = False,
+    with_: str = None,
+    conn=None,
 ) -> bool:
     """
     Checks if a given table exists for a given connection
 
     Parameters
     ----------
     table: str
@@ -59,23 +63,27 @@
         Avoid raising a ValueError
     """
     if table is None:
         if ignore_error:
             return False
         else:
             raise ValueError("Table cannot be None")
+    if not Connection.current:
+        raise RuntimeError("No active connection")
+    if not conn:
+        conn = Connection.current
 
     table = strip_multiple_chars(table, "\"'")
 
     if schema:
         table_ = f"{schema}.{table}"
     else:
         table_ = table
 
-    _is_exist = _is_table_exists(table_, with_)
+    _is_exist = _is_table_exists(table_, with_, conn)
 
     if not _is_exist:
         if not ignore_error:
             expected = []
             existing_schemas = inspect.get_schema_names()
             if schema and schema not in existing_schemas:
                 expected = existing_schemas
@@ -148,30 +156,32 @@
 def strip_multiple_chars(string: str, chars: str) -> str:
     """
     Trims characters from the start and end of the string
     """
     return string.translate(str.maketrans("", "", chars))
 
 
-def _is_table_exists(table: str, with_: str) -> bool:
+def _is_table_exists(table: str, with_: str, conn) -> bool:
     """
     Runs a SQL query to check if table exists
     """
-    identifiers = Connection.get_curr_identifiers()
+    if not conn:
+        conn = Connection.current
+    identifiers = conn.get_curr_identifiers()
     if with_:
         return table in list(store)
     else:
         for iden in identifiers:
             if isinstance(iden, tuple):
                 query = "SELECT * FROM {0}{1}{2} WHERE 1=0".format(
                     iden[0], table, iden[1]
                 )
             else:
                 query = "SELECT * FROM {0}{1}{0} WHERE 1=0".format(iden, table)
             try:
-                query = sql.connection.Connection._transpile_query(query)
-                sql.run.raw_run(Connection.current, query)
+                query = conn._transpile_query(query)
+                sql.run.raw_run(conn, query)
                 return True
             except Exception:
                 pass
 
     return False
```


# Comparing `tmp/gqlalchemy-1.4.0.tar.gz` & `tmp/gqlalchemy-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gqlalchemy-1.4.0.tar", max compression
+gzip compressed data, was "gqlalchemy-1.4.1.tar", max compression
```

## Comparing `gqlalchemy-1.4.0.tar` & `gqlalchemy-1.4.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0    10174 2022-03-23 14:14:35.637857 gqlalchemy-1.4.0/LICENSE
--rw-r--r--   0        0        0     9345 2022-12-01 19:12:02.074293 gqlalchemy-1.4.0/README.md
--rw-r--r--   0        0        0     2227 2022-09-09 17:31:38.518107 gqlalchemy-1.4.0/gqlalchemy/__init__.py
--rw-r--r--   0        0        0     1118 2022-12-20 14:58:12.495149 gqlalchemy-1.4.0/gqlalchemy/bruno_test_graph_algorithms.py
--rw-r--r--   0        0        0     1224 2022-12-01 14:39:45.305625 gqlalchemy-1.4.0/gqlalchemy/bruno_test_importer.py
--rw-r--r--   0        0        0      853 2022-09-02 14:04:39.047604 gqlalchemy-1.4.0/gqlalchemy/config.yml
--rw-r--r--   0        0        0     7524 2023-03-10 13:08:52.761492 gqlalchemy-1.4.0/gqlalchemy/connection.py
--rw-r--r--   0        0        0     8317 2022-09-09 17:31:38.518107 gqlalchemy-1.4.0/gqlalchemy/disk_storage.py
--rw-r--r--   0        0        0     7376 2022-12-01 19:12:02.078293 gqlalchemy-1.4.0/gqlalchemy/exceptions.py
--rw-r--r--   0        0        0      609 2022-09-09 17:31:38.518107 gqlalchemy-1.4.0/gqlalchemy/graph_algorithms/__init__.py
--rw-r--r--   0        0        0     9253 2023-03-10 13:08:52.765492 gqlalchemy-1.4.0/gqlalchemy/graph_algorithms/integrated_algorithms.py
--rw-r--r--   0        0        0    31176 2023-03-09 13:56:34.778051 gqlalchemy-1.4.0/gqlalchemy/graph_algorithms/query_builder.py
--rw-r--r--   0        0        0     5700 2022-09-09 17:31:38.518107 gqlalchemy-1.4.0/gqlalchemy/graph_algorithms/query_modules.py
--rw-r--r--   0        0        0     8354 2022-11-11 08:24:54.025229 gqlalchemy-1.4.0/gqlalchemy/instance_runner.py
--rw-r--r--   0        0        0      368 2023-03-10 13:08:52.765492 gqlalchemy-1.4.0/gqlalchemy/memgraph_constants.py
--rw-r--r--   0        0        0    24544 2022-12-01 19:12:02.078293 gqlalchemy-1.4.0/gqlalchemy/models.py
--rw-r--r--   0        0        0      609 2022-09-09 17:31:38.518107 gqlalchemy-1.4.0/gqlalchemy/query_builders/__init__.py
--rw-r--r--   0        0        0    57593 2023-03-10 13:08:52.765492 gqlalchemy-1.4.0/gqlalchemy/query_builders/declarative_base.py
--rw-r--r--   0        0        0     9552 2023-03-10 13:08:52.765492 gqlalchemy-1.4.0/gqlalchemy/query_builders/memgraph_query_builder.py
--rw-r--r--   0        0        0      961 2022-09-09 17:31:38.518107 gqlalchemy-1.4.0/gqlalchemy/query_builders/neo4j_query_builder.py
--rw-r--r--   0        0        0      609 2022-09-09 17:31:38.518107 gqlalchemy-1.4.0/gqlalchemy/query_modules/__init__.py
--rw-r--r--   0        0        0     2652 2022-09-09 17:31:38.522107 gqlalchemy-1.4.0/gqlalchemy/query_modules/push_streams/kafka.py
--rw-r--r--   0        0        0     2598 2022-09-09 17:31:38.522107 gqlalchemy-1.4.0/gqlalchemy/query_modules/push_streams/power_bi.py
--rw-r--r--   0        0        0        0 2023-03-10 13:08:52.765492 gqlalchemy-1.4.0/gqlalchemy/transformations/__init__.py
--rw-r--r--   0        0        0      263 2023-03-10 13:08:52.765492 gqlalchemy-1.4.0/gqlalchemy/transformations/constants.py
--rw-r--r--   0        0        0      609 2023-03-10 13:08:52.769492 gqlalchemy-1.4.0/gqlalchemy/transformations/export/__init__.py
--rw-r--r--   0        0        0     2761 2023-03-10 13:08:52.769492 gqlalchemy-1.4.0/gqlalchemy/transformations/export/graph_transporter.py
--rw-r--r--   0        0        0     1132 2023-03-10 13:08:52.769492 gqlalchemy-1.4.0/gqlalchemy/transformations/export/transporter.py
--rw-r--r--   0        0        0       75 2023-03-10 13:08:52.769492 gqlalchemy-1.4.0/gqlalchemy/transformations/graph_type.py
--rw-r--r--   0        0        0      609 2023-03-10 13:08:52.769492 gqlalchemy-1.4.0/gqlalchemy/transformations/importing/__init__.py
--rw-r--r--   0        0        0     2837 2023-03-10 13:08:52.769492 gqlalchemy-1.4.0/gqlalchemy/transformations/importing/graph_importer.py
--rw-r--r--   0        0        0      874 2023-03-10 13:08:52.769492 gqlalchemy-1.4.0/gqlalchemy/transformations/importing/importer.py
--rw-r--r--   0        0        0    38405 2023-03-10 13:08:52.769492 gqlalchemy-1.4.0/gqlalchemy/transformations/importing/loaders.py
--rw-r--r--   0        0        0      609 2023-03-10 13:08:52.769492 gqlalchemy-1.4.0/gqlalchemy/transformations/translators/__init__.py
--rw-r--r--   0        0        0     7953 2023-03-10 13:08:52.773491 gqlalchemy-1.4.0/gqlalchemy/transformations/translators/dgl_translator.py
--rw-r--r--   0        0        0    11648 2023-03-10 13:08:52.773491 gqlalchemy-1.4.0/gqlalchemy/transformations/translators/nx_translator.py
--rw-r--r--   0        0        0     9217 2023-03-10 13:08:52.773491 gqlalchemy-1.4.0/gqlalchemy/transformations/translators/pyg_translator.py
--rw-r--r--   0        0        0     9610 2023-03-10 13:08:52.773491 gqlalchemy-1.4.0/gqlalchemy/transformations/translators/translator.py
--rw-r--r--   0        0        0     6994 2023-03-10 13:08:52.773491 gqlalchemy-1.4.0/gqlalchemy/utilities.py
--rw-r--r--   0        0        0      609 2022-09-09 17:31:38.522107 gqlalchemy-1.4.0/gqlalchemy/vendors/__init__.py
--rw-r--r--   0        0        0    13131 2023-03-10 13:08:52.773491 gqlalchemy-1.4.0/gqlalchemy/vendors/database_client.py
--rw-r--r--   0        0        0    17869 2023-03-10 13:08:52.773491 gqlalchemy-1.4.0/gqlalchemy/vendors/memgraph.py
--rw-r--r--   0        0        0     9089 2022-09-09 17:31:38.522107 gqlalchemy-1.4.0/gqlalchemy/vendors/neo4j.py
--rw-r--r--   0        0        0     1416 2023-03-10 15:11:28.438022 gqlalchemy-1.4.0/pyproject.toml
--rw-r--r--   0        0        0    10939 1970-01-01 00:00:00.000000 gqlalchemy-1.4.0/setup.py
--rw-r--r--   0        0        0    10560 1970-01-01 00:00:00.000000 gqlalchemy-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0    10174 2022-03-23 14:14:35.637857 gqlalchemy-1.4.1/LICENSE
+-rw-r--r--   0        0        0    10756 2023-04-19 08:46:34.142380 gqlalchemy-1.4.1/README.md
+-rw-r--r--   0        0        0     2227 2022-09-09 17:31:38.518107 gqlalchemy-1.4.1/gqlalchemy/__init__.py
+-rw-r--r--   0        0        0      125 2023-04-04 09:44:45.940746 gqlalchemy-1.4.1/gqlalchemy/address.csv
+-rw-r--r--   0        0        0     1118 2022-12-20 14:58:12.495149 gqlalchemy-1.4.1/gqlalchemy/bruno_test_graph_algorithms.py
+-rw-r--r--   0        0        0     1224 2022-12-01 14:39:45.305625 gqlalchemy-1.4.1/gqlalchemy/bruno_test_importer.py
+-rw-r--r--   0        0        0      850 2023-04-04 09:46:13.803010 gqlalchemy-1.4.1/gqlalchemy/config.yml
+-rw-r--r--   0        0        0     7524 2023-03-10 13:08:52.761492 gqlalchemy-1.4.1/gqlalchemy/connection.py
+-rw-r--r--   0        0        0     8317 2022-09-09 17:31:38.518107 gqlalchemy-1.4.1/gqlalchemy/disk_storage.py
+-rw-r--r--   0        0        0     7635 2023-04-19 08:46:34.158380 gqlalchemy-1.4.1/gqlalchemy/exceptions.py
+-rw-r--r--   0        0        0      609 2022-09-09 17:31:38.518107 gqlalchemy-1.4.1/gqlalchemy/graph_algorithms/__init__.py
+-rw-r--r--   0        0        0     9253 2023-03-10 13:08:52.765492 gqlalchemy-1.4.1/gqlalchemy/graph_algorithms/integrated_algorithms.py
+-rw-r--r--   0        0        0    31176 2023-03-09 13:56:34.778051 gqlalchemy-1.4.1/gqlalchemy/graph_algorithms/query_builder.py
+-rw-r--r--   0        0        0     5700 2022-09-09 17:31:38.518107 gqlalchemy-1.4.1/gqlalchemy/graph_algorithms/query_modules.py
+-rw-r--r--   0        0        0      115 2023-04-04 09:44:45.940746 gqlalchemy-1.4.1/gqlalchemy/individual.csv
+-rw-r--r--   0        0        0     8354 2022-11-11 08:24:54.025229 gqlalchemy-1.4.1/gqlalchemy/instance_runner.py
+-rw-r--r--   0        0        0      368 2023-03-10 13:08:52.765492 gqlalchemy-1.4.1/gqlalchemy/memgraph_constants.py
+-rw-r--r--   0        0        0    24532 2023-04-19 08:46:34.158380 gqlalchemy-1.4.1/gqlalchemy/models.py
+-rw-r--r--   0        0        0      609 2022-09-09 17:31:38.518107 gqlalchemy-1.4.1/gqlalchemy/query_builders/__init__.py
+-rw-r--r--   0        0        0    57593 2023-03-10 13:08:52.765492 gqlalchemy-1.4.1/gqlalchemy/query_builders/declarative_base.py
+-rw-r--r--   0        0        0     9552 2023-03-10 13:08:52.765492 gqlalchemy-1.4.1/gqlalchemy/query_builders/memgraph_query_builder.py
+-rw-r--r--   0        0        0      961 2022-09-09 17:31:38.518107 gqlalchemy-1.4.1/gqlalchemy/query_builders/neo4j_query_builder.py
+-rw-r--r--   0        0        0      609 2022-09-09 17:31:38.518107 gqlalchemy-1.4.1/gqlalchemy/query_modules/__init__.py
+-rw-r--r--   0        0        0     2652 2022-09-09 17:31:38.522107 gqlalchemy-1.4.1/gqlalchemy/query_modules/push_streams/kafka.py
+-rw-r--r--   0        0        0     2598 2022-09-09 17:31:38.522107 gqlalchemy-1.4.1/gqlalchemy/query_modules/push_streams/power_bi.py
+-rw-r--r--   0        0        0        0 2023-03-10 13:08:52.765492 gqlalchemy-1.4.1/gqlalchemy/transformations/__init__.py
+-rw-r--r--   0        0        0      263 2023-03-10 13:08:52.765492 gqlalchemy-1.4.1/gqlalchemy/transformations/constants.py
+-rw-r--r--   0        0        0      609 2023-03-10 13:08:52.769492 gqlalchemy-1.4.1/gqlalchemy/transformations/export/__init__.py
+-rw-r--r--   0        0        0     3122 2023-04-19 08:46:34.158380 gqlalchemy-1.4.1/gqlalchemy/transformations/export/graph_transporter.py
+-rw-r--r--   0        0        0     1132 2023-03-10 13:08:52.769492 gqlalchemy-1.4.1/gqlalchemy/transformations/export/transporter.py
+-rw-r--r--   0        0        0       75 2023-03-10 13:08:52.769492 gqlalchemy-1.4.1/gqlalchemy/transformations/graph_type.py
+-rw-r--r--   0        0        0      609 2023-03-10 13:08:52.769492 gqlalchemy-1.4.1/gqlalchemy/transformations/importing/__init__.py
+-rw-r--r--   0        0        0     3199 2023-04-19 08:46:34.158380 gqlalchemy-1.4.1/gqlalchemy/transformations/importing/graph_importer.py
+-rw-r--r--   0        0        0      874 2023-03-10 13:08:52.769492 gqlalchemy-1.4.1/gqlalchemy/transformations/importing/importer.py
+-rw-r--r--   0        0        0    38781 2023-04-19 08:46:34.158380 gqlalchemy-1.4.1/gqlalchemy/transformations/importing/loaders.py
+-rw-r--r--   0        0        0      609 2023-03-10 13:08:52.769492 gqlalchemy-1.4.1/gqlalchemy/transformations/translators/__init__.py
+-rw-r--r--   0        0        0     7953 2023-04-19 08:46:34.158380 gqlalchemy-1.4.1/gqlalchemy/transformations/translators/dgl_translator.py
+-rw-r--r--   0        0        0    11648 2023-03-10 13:08:52.773491 gqlalchemy-1.4.1/gqlalchemy/transformations/translators/nx_translator.py
+-rw-r--r--   0        0        0     9217 2023-03-10 13:08:52.773491 gqlalchemy-1.4.1/gqlalchemy/transformations/translators/pyg_translator.py
+-rw-r--r--   0        0        0     9793 2023-04-19 08:46:34.158380 gqlalchemy-1.4.1/gqlalchemy/transformations/translators/translator.py
+-rw-r--r--   0        0        0     7435 2023-04-19 08:46:34.158380 gqlalchemy-1.4.1/gqlalchemy/utilities.py
+-rw-r--r--   0        0        0      609 2022-09-09 17:31:38.522107 gqlalchemy-1.4.1/gqlalchemy/vendors/__init__.py
+-rw-r--r--   0        0        0    13131 2023-03-10 13:08:52.773491 gqlalchemy-1.4.1/gqlalchemy/vendors/database_client.py
+-rw-r--r--   0        0        0    17869 2023-03-10 13:08:52.773491 gqlalchemy-1.4.1/gqlalchemy/vendors/memgraph.py
+-rw-r--r--   0        0        0     9089 2022-09-09 17:31:38.522107 gqlalchemy-1.4.1/gqlalchemy/vendors/neo4j.py
+-rw-r--r--   0        0        0     1655 2023-04-19 08:46:34.158380 gqlalchemy-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0    12181 1970-01-01 00:00:00.000000 gqlalchemy-1.4.1/PKG-INFO
```

### Comparing `gqlalchemy-1.4.0/LICENSE` & `gqlalchemy-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/README.md` & `gqlalchemy-1.4.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,41 +10,76 @@
     <a href="https://github.com/memgraph/gqlalchemy/stargazers" alt="Stargazers"><img src="https://img.shields.io/github/stars/memgraph/gqlalchemy?style=social" /></a>
 </p>
 
 **GQLAlchemy** is a fully open-source Python library and **Object Graph Mapper** (OGM) - a link between graph database objects and Python objects.
 
 An Object Graph Mapper or OGM provides a developer-friendly workflow that allows for writing object-oriented notation to communicate with graph databases. Instead of writing Cypher queries, you will be able to write object-oriented code, which the OGM will automatically translate into Cypher queries.
 
+## Installation
+
 GQLAlchemy is built on top of Memgraph's low-level Python client `pymgclient`
 ([PyPI](https://pypi.org/project/pymgclient/) /
 [Documentation](https://memgraph.github.io/pymgclient/) /
-[GitHub](https://github.com/memgraph/pymgclient)).
+[GitHub](https://github.com/memgraph/pymgclient)). 
 
-## Installation
+To install GQLAlchemy, you first need to install `pymgclient` [build prerequisites](https://memgraph.github.io/pymgclient/introduction.html#build-prerequisites).
 
-Before you install `gqlalchemy`, make sure that you have `cmake` installed by running:
-```
-cmake --version
-```
-You can install `cmake` by following the [official instructions](https://cgold.readthedocs.io/en/latest/first-step/installation.html#).
+After you have installed the prerequisites, run the following command:
 
-To install `gqlalchemy`, simply run the following command:
-```
-pip install gqlalchemy
+`pip install gqlalchemy`
+
+With the above command, you get the basic GQLAlchemy capabilities. To add additional import/export capabilities, install GQLAlchemy with one of the following commands:
+
+- `pip install gqlalchemy[arrow]` # Support for the CSV, Parquet, ORC and IPC/Feather/Arrow formats
+- `pip install gqlalchemy[dgl]` # DGL support (includes PyTorch)
+
+- `pip install gqlalchemy[all]` # All of the above
+
+If you intend to use GQLAlchemy with PyTorch Geometric support, that library must be installed manually:
+
+```bash
+pip install gqlalchemy[torch_pyg] # prerequisite
+pip install torch-scatter torch-sparse torch-cluster torch-spline-conv torch-geometric -f https://data.pyg.org/whl/torch-1.13.0+cpu.html"
 ```
 
 If you are using [Conda](https://docs.conda.io/en/latest/) for Python environment management, you can install GQLAlchemy through pip.
 
 ## Build & Test
 
-The project uses [Poetry](https://python-poetry.org/) to build the GQLAlchemy Python library. To build and run tests, execute the following command:
-`poetry install`
+The project uses [Poetry](https://python-poetry.org/) to build the library. Clone or download the [GQLAlchemy source code](https://github.com/memgraph/gqlalchemy) locally and run the following command to build it from source with Poetry:
+
+```bash
+poetry install --all-extras
+```
 
-Before starting the tests, make sure you have an active Memgraph instance running. Execute the following command:
-`poetry run pytest .`
+The ``poetry install --all-extras`` command installs GQLAlchemy with all extras
+(optional dependencies). Alternatively, you can use the ``-E`` option to define
+what extras to install:
+
+```bash
+poetry install # No extras
+
+poetry install -E arrow # Support for the CSV, Parquet, ORC and IPC/Feather/Arrow formats
+poetry install -E dgl # DGL support (also includes torch)
+```
+
+To run the tests, make sure you have an [active Memgraph instance](/memgraph), and execute one of the following commands:
+
+```bash
+poetry run pytest . -k "not slow" # If all extras installed
+
+poetry run pytest . -k "not slow and not extras" # Otherwise
+```
+
+If you’ve installed only certain extras, it’s also possible to run their associated tests:
+
+```bash
+poetry run pytest . -k "arrow"
+poetry run pytest . -k "dgl"
+```
 
 ## GQLAlchemy capabilities
 
 <details>
 <summary>🗺️ Object graph mapper</summary>
 <br>
 
@@ -231,28 +266,29 @@
 </details>
 
 <br>
 
 If you want to learn more about OGM, query builder, managing streams, importing data from different source, managing Memgraph instances, managing database triggers and using on-disk storage, check out the GQLAlchemy [how-to guides](https://memgraph.com/docs/gqlalchemy/how-to-guides).
 
 ## Development (how to build)
-```
+
+```bash
 poetry run flake8 .
 poetry run black .
-poetry run pytest . -k "not slow"
+poetry run pytest . -k "not slow and not extras"
 ```
 
 ## Documentation
 
 The GQLAlchemy documentation is available on [memgraph.com/docs/gqlalchemy](https://memgraph.com/docs/gqlalchemy/).
 
 The documentation can be generated by executing:
 ```
-pip3 install python-markdown
-python-markdown
+pip3 install pydoc-markdown
+pydoc-markdown
 ```
 
 ## License
 
 Copyright (c) 2016-2022 [Memgraph Ltd.](https://memgraph.com)
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not use
```

### Comparing `gqlalchemy-1.4.0/gqlalchemy/__init__.py` & `gqlalchemy-1.4.1/gqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/bruno_test_graph_algorithms.py` & `gqlalchemy-1.4.1/gqlalchemy/bruno_test_graph_algorithms.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/bruno_test_importer.py` & `gqlalchemy-1.4.1/gqlalchemy/bruno_test_importer.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/config.yml` & `gqlalchemy-1.4.1/gqlalchemy/config.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 indices:    # indices to be created for each table
-  individuals:    # name of the table containing individuals with ind_id
+  individual:    # name of the table containing individuals with ind_id
   - ind_id
   address:
   - add_id
  
  
 name_mappings:    # how we want to name node labels
-  individuals:
+  individual:
     label: INDIVIDUAL    # nodes made from the individuals table will have the label INDIVIDUAL
   address:
     label: ADDRESS
  
  
 one_to_many_relations:
   address: []    # currently needed, leave [] if no relations to define
-  individuals:
+  individual:
   - foreign_key:                # foreign key used for mapping;
       column_name: add_id         # specifies its column
       reference_table: address    # name of table from which the foreign key is taken
       reference_key: add_id       # column name in reference table from which the foreign key is taken
     label: LIVES_IN               # label applied to relationship created
```

### Comparing `gqlalchemy-1.4.0/gqlalchemy/connection.py` & `gqlalchemy-1.4.1/gqlalchemy/connection.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/disk_storage.py` & `gqlalchemy-1.4.1/gqlalchemy/disk_storage.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/exceptions.py` & `gqlalchemy-1.4.1/gqlalchemy/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,18 @@
 
 from gqlalchemy import Memgraph, SQLitePropertyDatabase
 
 db = Memgraph()
 SQLitePropertyDatabase("path-to-sqlite-db", db)
 """
 
+MISSING_OPTIONAL_DEPENDENCY = """
+No module named '{dependency_name}'
+"""
+
 MISSING_ORDER = """
 The second argument of the tuple must be order: ASC, ASCENDING, DESC or DESCENDING.
 """
 
 ORDER_BY_TYPE_ERROR = """
 TypeError: The argument provided is of wrong type. Please provide str, tuple[str, str] or list[tuple[str, str]].
 """
@@ -195,14 +199,19 @@
 
 class GQLAlchemyFileNotFoundError(GQLAlchemyError):
     def __init__(self, path):
         super().__init__()
         self.message = FILE_NOT_FOUND.format(path=path)
 
 
+def raise_if_not_imported(dependency, dependency_name):
+    if not dependency:
+        raise ModuleNotFoundError(MISSING_OPTIONAL_DEPENDENCY.format(dependency_name=dependency_name))
+
+
 def database_error_handler(func):
     def inner_function(*args, **kwargs):
         try:
             return func(*args, **kwargs)
         except Exception as e:
             raise GQLAlchemyDatabaseError(e) from e
```

### Comparing `gqlalchemy-1.4.0/gqlalchemy/graph_algorithms/__init__.py` & `gqlalchemy-1.4.1/gqlalchemy/graph_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/graph_algorithms/integrated_algorithms.py` & `gqlalchemy-1.4.1/gqlalchemy/graph_algorithms/integrated_algorithms.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/graph_algorithms/query_builder.py` & `gqlalchemy-1.4.1/gqlalchemy/graph_algorithms/query_builder.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/graph_algorithms/query_modules.py` & `gqlalchemy-1.4.1/gqlalchemy/graph_algorithms/query_modules.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/instance_runner.py` & `gqlalchemy-1.4.1/gqlalchemy/instance_runner.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/models.py` & `gqlalchemy-1.4.1/gqlalchemy/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,17 +370,17 @@
         elif value_type == int:
             return repr(value)
         elif value_type == float:
             return repr(value)
         elif isinstance(value, str):
             return repr(value) if value.isprintable() else rf"'{value}'"
         elif isinstance(value, list):
-            return "[" + ", ".join(self.escape_value(val, True) for val in value) + "]"
+            return "[" + ", ".join(self.escape_value(val) for val in value) + "]"
         elif value_type == dict:
-            return "{" + ", ".join(f"{val}: {self.escape_value(val, True)}" for key, val in value.items()) + "}"
+            return "{" + ", ".join(f"{key}: {self.escape_value(val)}" for key, val in value.items()) + "}"
         if isinstance(value, (timedelta, time, datetime, date)):
             return f"{datetimeKwMapping[value_type]}('{_format_timedelta(value) if isinstance(value, timedelta) else value.isoformat()}')"
         else:
             raise GQLAlchemyError(
                 f"Unsupported value data type: {type(value)}."
                 + " Memgraph supports the following data types:"
                 + " None, bool, int, float, str, list, dict, datetime."
```

### Comparing `gqlalchemy-1.4.0/gqlalchemy/query_builders/__init__.py` & `gqlalchemy-1.4.1/gqlalchemy/query_builders/__init__.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/query_builders/declarative_base.py` & `gqlalchemy-1.4.1/gqlalchemy/query_builders/declarative_base.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/query_builders/memgraph_query_builder.py` & `gqlalchemy-1.4.1/gqlalchemy/query_builders/memgraph_query_builder.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/query_builders/neo4j_query_builder.py` & `gqlalchemy-1.4.1/gqlalchemy/query_builders/neo4j_query_builder.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/query_modules/__init__.py` & `gqlalchemy-1.4.1/gqlalchemy/query_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/query_modules/push_streams/kafka.py` & `gqlalchemy-1.4.1/gqlalchemy/query_modules/push_streams/kafka.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/query_modules/push_streams/power_bi.py` & `gqlalchemy-1.4.1/gqlalchemy/query_modules/push_streams/power_bi.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/transformations/export/__init__.py` & `gqlalchemy-1.4.1/gqlalchemy/transformations/export/__init__.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/transformations/export/graph_transporter.py` & `gqlalchemy-1.4.1/gqlalchemy/transformations/export/graph_transporter.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,20 +8,30 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from gqlalchemy.exceptions import raise_if_not_imported
+import gqlalchemy.memgraph_constants as mg_consts
 from gqlalchemy.transformations.export.transporter import Transporter
-from gqlalchemy.transformations.translators.dgl_translator import DGLTranslator
-from gqlalchemy.transformations.translators.nx_translator import NxTranslator
-from gqlalchemy.transformations.translators.pyg_translator import PyGTranslator
 from gqlalchemy.transformations.graph_type import GraphType
-import gqlalchemy.memgraph_constants as mg_consts
+
+try:
+    from gqlalchemy.transformations.translators.dgl_translator import DGLTranslator
+except ModuleNotFoundError:
+    DGLTranslator = None
+
+from gqlalchemy.transformations.translators.nx_translator import NxTranslator
+
+try:
+    from gqlalchemy.transformations.translators.pyg_translator import PyGTranslator
+except ModuleNotFoundError:
+    PyGTranslator = None
 
 
 class GraphTransporter(Transporter):
     """Here is a possible example for using this module:
     >>> transporter = GraphTransporter("dgl")
     graph = transporter.export()
     """
@@ -43,16 +53,18 @@
         graph = transporter.export()
         Args:
             graph_type: dgl, pyg or nx
         """
         super().__init__()
         self.graph_type = graph_type.upper()
         if self.graph_type == GraphType.DGL.name:
+            raise_if_not_imported(dependency=DGLTranslator, dependency_name="dgl")
             self.translator = DGLTranslator(host, port, username, password, encrypted, client_name, lazy)
         elif self.graph_type == GraphType.PYG.name:
+            raise_if_not_imported(dependency=PyGTranslator, dependency_name="torch_geometric")
             self.translator = PyGTranslator(host, port, username, password, encrypted, client_name, lazy)
         elif self.graph_type == GraphType.NX.name:
             self.translator = NxTranslator(host, port, username, password, encrypted, client_name, lazy)
         else:
             raise ValueError("Unknown export option. Currently supported are DGL, PyG and Networkx.")
 
     def export(self):
```

### Comparing `gqlalchemy-1.4.0/gqlalchemy/transformations/export/transporter.py` & `gqlalchemy-1.4.1/gqlalchemy/transformations/export/transporter.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/transformations/importing/__init__.py` & `gqlalchemy-1.4.1/gqlalchemy/transformations/importing/__init__.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/transformations/importing/graph_importer.py` & `gqlalchemy-1.4.1/gqlalchemy/transformations/importing/graph_importer.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,19 +11,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from gqlalchemy import Memgraph
 from gqlalchemy.transformations.graph_type import GraphType
 from gqlalchemy.transformations.importing.importer import Importer
-from gqlalchemy.transformations.translators.dgl_translator import DGLTranslator
-from gqlalchemy.transformations.translators.nx_translator import NxTranslator
-from gqlalchemy.transformations.translators.pyg_translator import PyGTranslator
+
+from gqlalchemy.exceptions import raise_if_not_imported
 import gqlalchemy.memgraph_constants as mg_consts
 
+try:
+    from gqlalchemy.transformations.translators.dgl_translator import DGLTranslator
+except ModuleNotFoundError:
+    DGLTranslator = None
+
+from gqlalchemy.transformations.translators.nx_translator import NxTranslator
+
+try:
+    from gqlalchemy.transformations.translators.pyg_translator import PyGTranslator
+except ModuleNotFoundError:
+    PyGTranslator = None
+
 
 class GraphImporter(Importer):
     """Imports dgl, pyg or networkx graph representations to Memgraph.
     The following code will suffice for importing queries.
     >>> importer = GraphImporter("dgl")
     graph = DGLGraph(...)
     importer.translate(graph)  # queries are inserted in this step
@@ -41,16 +52,18 @@
         encrypted: bool = mg_consts.MG_ENCRYPTED,
         client_name: str = mg_consts.MG_CLIENT_NAME,
         lazy: bool = mg_consts.MG_LAZY,
     ) -> None:
         super().__init__()
         self.graph_type = graph_type.upper()
         if self.graph_type == GraphType.DGL.name:
+            raise_if_not_imported(dependency=DGLTranslator, dependency_name="dgl")
             self.translator = DGLTranslator(host, port, username, password, encrypted, client_name, lazy)
         elif self.graph_type == GraphType.PYG.name:
+            raise_if_not_imported(dependency=PyGTranslator, dependency_name="torch_geometric")
             self.translator = PyGTranslator(host, port, username, password, encrypted, client_name, lazy)
         elif self.graph_type == GraphType.NX.name:
             self.translator = NxTranslator(host, port, username, password, encrypted, client_name, lazy)
         else:
             raise ValueError("Unknown import option. Currently supported options are: DGL, PyG and Networkx.")
 
     def translate(self, graph) -> None:
```

### Comparing `gqlalchemy-1.4.0/gqlalchemy/transformations/importing/importer.py` & `gqlalchemy-1.4.1/gqlalchemy/transformations/importing/importer.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/transformations/importing/loaders.py` & `gqlalchemy-1.4.1/gqlalchemy/transformations/importing/loaders.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,23 @@
 from abc import ABC, abstractmethod
 from enum import Enum
 from dataclasses import dataclass, field
 from string import Template
 from typing import List, Dict, Any, Optional, Union
 
 import adlfs
-import pyarrow.dataset as ds
-from pyarrow import fs
+
+try:
+    import pyarrow.dataset as ds
+except ModuleNotFoundError:
+    ds = None
+try:
+    from pyarrow import fs
+except ModuleNotFoundError:
+    fs = None
 from dacite import from_dict
 
 from gqlalchemy import Memgraph
 from gqlalchemy.models import (
     MemgraphIndex,
     MemgraphTrigger,
     TriggerEventObject,
@@ -219,14 +226,17 @@
             KeyError: kwargs doesn't contain necessary fields.
         """
         if S3_ACCESS_KEY not in kwargs:
             raise KeyError(f"{S3_ACCESS_KEY} is needed to connect to S3 storage")
         if S3_SECRET_KEY not in kwargs:
             raise KeyError(f"{S3_SECRET_KEY} is needed to connect to S3 storage")
 
+        if fs is None:
+            raise ModuleNotFoundError("No module named 'pyarrow'")
+
         super().__init__(fs=fs.S3FileSystem(**kwargs))
         self._bucket_name = bucket_name
 
     def get_path(self, collection_name: str) -> str:
         """Get file path in file system.
 
         Args:
@@ -274,14 +284,17 @@
 
     def __init__(self, path: str) -> None:
         """Initializes an fsspec local file system and sets path to data.
 
         Args:
             path: path to the local storage location.
         """
+        if fs is None:
+            raise ModuleNotFoundError("No module named 'pyarrow'")
+
         super().__init__(fs=fs.LocalFileSystem())
         self._path = path
 
     def get_path(self, collection_name: str) -> str:
         """Get file path in the local file system.
 
         Args:
@@ -357,14 +370,17 @@
             collection_name: Name of the file to read.
             is_cross_table: Flag signifying whether it is a cross table.
             columns: Table columns to read.
         """
         source = self._file_system_handler.get_path(f"{collection_name}.{self._file_extension}")
         print("Loading data from " + ("cross " if is_cross_table else "") + f"table {source}...")
 
+        if ds is None:
+            raise ModuleNotFoundError("No module named 'pyarrow'")
+
         dataset = ds.dataset(source=source, format=self._file_extension, filesystem=self._file_system_handler.fs)
 
         for batch in dataset.to_batches(
             columns=columns,
         ):
             for batch_item in batch.to_pylist():
                 yield batch_item
```

### Comparing `gqlalchemy-1.4.0/gqlalchemy/transformations/translators/__init__.py` & `gqlalchemy-1.4.1/gqlalchemy/transformations/translators/__init__.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/transformations/translators/dgl_translator.py` & `gqlalchemy-1.4.1/gqlalchemy/transformations/translators/dgl_translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 )
 
 
 class DGLTranslator(Translator):
     """Performs conversion from cypher queries to the DGL graph representation. DGL assigns to each edge a unique integer, called the edge ID,
     based on the order in which it was added to the graph. In DGL, all the edges are directed, and an edge (u,v) indicates that the direction goes
     from node u to node v. Only features of numerical types (e.g., float, double, and int) are allowed. They can be scalars, vectors or multi-dimensional
-    tensors (DQL requirement). Each node feature has a unique name and each edge feature has a unique name. The features of nodes and edges can have
+    tensors (DGL requirement). Each node feature has a unique name and each edge feature has a unique name. The features of nodes and edges can have
     the same name. A feature is created via tensor assignment, which assigns a feature to each node/edge in the graph. The leading dimension of that
     tensor must be equal to the number of nodes/edges in the graph. You cannot assign a feature to a subset of the nodes/edges in the graph. Features of the
     same name must have the same dimensionality and data type.
     """
 
     def __init__(
         self,
```

### Comparing `gqlalchemy-1.4.0/gqlalchemy/transformations/translators/nx_translator.py` & `gqlalchemy-1.4.1/gqlalchemy/transformations/translators/nx_translator.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/transformations/translators/pyg_translator.py` & `gqlalchemy-1.4.1/gqlalchemy/transformations/translators/pyg_translator.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/transformations/translators/translator.py` & `gqlalchemy-1.4.1/gqlalchemy/transformations/translators/translator.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,20 @@
 # limitations under the License.
 
 from abc import ABC, abstractmethod
 from typing import Callable, List, Set, Dict, Tuple
 from collections import defaultdict
 from numbers import Number
 
-import torch
+try:
+    import torch
+except ModuleNotFoundError:
+    torch = None
 
+from gqlalchemy.exceptions import raise_if_not_imported
 from gqlalchemy.transformations.constants import LABELS_CONCAT, DEFAULT_NODE_LABEL, DEFAULT_EDGE_TYPE
 from gqlalchemy.memgraph_constants import (
     MG_HOST,
     MG_PORT,
     MG_USERNAME,
     MG_PASSWORD,
     MG_ENCRYPTED,
@@ -31,15 +35,14 @@
 )
 from gqlalchemy.models import Node, Relationship
 from gqlalchemy.utilities import to_cypher_properties
 from gqlalchemy import Memgraph, Match
 
 
 class Translator(ABC):
-
     # Lambda function to concat list of labels
     merge_labels: Callable[[Set[str]], str] = (
         lambda labels, default_node_label: LABELS_CONCAT.join([label for label in sorted(labels)])
         if len(labels)
         else default_node_label
     )
 
@@ -100,14 +103,16 @@
         """Return true if features are okay to be set on all nodes/features.
         Args:
             features: To be set on all nodes. It can be anything that can be converted to torch tensor.
             expected_num: This can be number of nodes or number of edges depending on whether features will be set on nodes or edges.
         Returns:
             None if features cannot be set or tensor of same features.
         """
+        raise_if_not_imported(dependency=torch, dependency_name="torch")
+
         if len(features) != expected_num:
             return None
         try:
             return torch.tensor(features, dtype=torch.float32)
         except ValueError:
             return None
```

### Comparing `gqlalchemy-1.4.0/gqlalchemy/utilities.py` & `gqlalchemy-1.4.1/gqlalchemy/utilities.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,22 +9,29 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from abc import ABC, abstractmethod
-import math
-import numpy as np
-import torch
-
 from datetime import datetime, date, time, timedelta
 from enum import Enum
+import inspect
+import math
 from typing import Any, Dict, List, Optional, Tuple, Union
 
+import numpy as np
+
+try:
+    import torch
+except ModuleNotFoundError:
+    torch = None
+
+from gqlalchemy.exceptions import raise_if_not_imported
+
 
 class DatetimeKeywords(Enum):
     DURATION = "duration"
     LOCALTIME = "localTime"
     LOCALDATETIME = "localDateTime"
     DATE = "date"
 
@@ -63,21 +70,34 @@
     remainder_sec -= hours * 3600
     minutes = int(remainder_sec // 60)
     remainder_sec -= minutes * 60
 
     return f"P{days}DT{hours}H{minutes}M{remainder_sec}S"
 
 
+def _is_torch_tensor(value):
+    for cls in inspect.getmro(type(value)):
+        try:
+            if cls.__module__ == "torch" and cls.__name__ == "Tensor":
+                return True
+        except Exception:
+            pass
+    return False
+
+
 def to_cypher_value(value: Any, config: NetworkXCypherConfig = None) -> str:
     """Converts value to a valid Cypher type."""
     if config is None:
         config = NetworkXCypherConfig()
 
     value_type = type(value)
-    if isinstance(value, torch.Tensor):
+
+    if _is_torch_tensor(value):
+        raise_if_not_imported(dependency=torch, dependency_name="torch")
+
         if value.squeeze().size() == 1:
             return value.squeeze().item()
         else:
             return value.tolist()
 
     if isinstance(value_type, str) and is_numeric(value):
         return float(value)
```

### Comparing `gqlalchemy-1.4.0/gqlalchemy/vendors/__init__.py` & `gqlalchemy-1.4.1/gqlalchemy/vendors/__init__.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/vendors/database_client.py` & `gqlalchemy-1.4.1/gqlalchemy/vendors/database_client.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/vendors/memgraph.py` & `gqlalchemy-1.4.1/gqlalchemy/vendors/memgraph.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/gqlalchemy/vendors/neo4j.py` & `gqlalchemy-1.4.1/gqlalchemy/vendors/neo4j.py`

 * *Files identical despite different names*

### Comparing `gqlalchemy-1.4.0/pyproject.toml` & `gqlalchemy-1.4.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "GQLAlchemy"
-version = "1.4.0"
+version = "1.4.1"
 
-description = "GQLAlchemy is library developed with purpose of assisting writing and running queries on Memgraph."
+description = "GQLAlchemy is a library developed to assist with writing and running queries in Memgraph."
 repository = "https://github.com/memgraph/gqlalchemy"
 authors = [
-    "Bruno Sacaric <bruno.sacaric@memgraph.com>",
-    "Josip Mrden <josip.mrden@memgraph.com>",
-    "Katarina Supe <katarina.supe@memgraph.com>",
-    "Andi Skrgat <andi.skrgat@memgraph.com>",
+  "Bruno Sacaric <bruno.sacaric@memgraph.com>",
+  "Josip Mrden <josip.mrden@memgraph.com>",
+  "Katarina Supe <katarina.supe@memgraph.com>",
+  "Andi Skrgat <andi.skrgat@memgraph.com>",
+  "Ante Pusic <ante.pusic@memgraph.io>",
 ]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "gqlalchemy" }]
 
 [tool.black]
 line-length = 120
@@ -33,22 +34,29 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pymgclient = "1.3.1"
 networkx = "^2.5.1"
 pydantic = "^1.8.2"
 psutil = "^5.9.0"
-pyarrow = "^9.0.0"
 dacite = "^1.6.0"
 adlfs = "^2022.2.0"
 neo4j = "^4.4.3"
-docker = "^5.0.3"
-torch = "^1.13.1"
 numpy = "^1.24.1"
-dgl = "^0.9.1"
+docker = "^5.0.3"
+
+pyarrow = { version = "^9.0.0", optional = true }
+torch = { version = "^1.13.1", optional = true }
+dgl = { version = "^0.9.1", optional = true }
+
+[tool.poetry.extras]
+arrow = ["pyarrow"]
+dgl = ["torch", "dgl"]
+all = ["pyarrow", "torch", "dgl"]
+torch_pyg = ["torch"]
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.3.0"
 pytest = "^7.1.1"
 pytest-black = "^0.3.12"
 pytest-cov = "^2.12.0"
 pytest-flake8 = "1.0.7"
```

### Comparing `gqlalchemy-1.4.0/setup.py` & `gqlalchemy-1.4.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,684 +1,762 @@
-00000000: 2320 2d2a 2d20 636f 6469 6e67 3a20 7574  # -*- coding: ut
-00000010: 662d 3820 2d2a 2d0a 6672 6f6d 2073 6574  f-8 -*-.from set
-00000020: 7570 746f 6f6c 7320 696d 706f 7274 2073  uptools import s
-00000030: 6574 7570 0a0a 7061 636b 6167 6573 203d  etup..packages =
-00000040: 205c 0a5b 2767 716c 616c 6368 656d 7927   \.['gqlalchemy'
-00000050: 2c0a 2027 6771 6c61 6c63 6865 6d79 2e67  ,. 'gqlalchemy.g
-00000060: 7261 7068 5f61 6c67 6f72 6974 686d 7327  raph_algorithms'
-00000070: 2c0a 2027 6771 6c61 6c63 6865 6d79 2e71  ,. 'gqlalchemy.q
-00000080: 7565 7279 5f62 7569 6c64 6572 7327 2c0a  uery_builders',.
-00000090: 2027 6771 6c61 6c63 6865 6d79 2e71 7565   'gqlalchemy.que
-000000a0: 7279 5f6d 6f64 756c 6573 272c 0a20 2767  ry_modules',. 'g
-000000b0: 716c 616c 6368 656d 792e 7175 6572 795f  qlalchemy.query_
-000000c0: 6d6f 6475 6c65 732e 7075 7368 5f73 7472  modules.push_str
-000000d0: 6561 6d73 272c 0a20 2767 716c 616c 6368  eams',. 'gqlalch
-000000e0: 656d 792e 7472 616e 7366 6f72 6d61 7469  emy.transformati
-000000f0: 6f6e 7327 2c0a 2027 6771 6c61 6c63 6865  ons',. 'gqlalche
-00000100: 6d79 2e74 7261 6e73 666f 726d 6174 696f  my.transformatio
-00000110: 6e73 2e65 7870 6f72 7427 2c0a 2027 6771  ns.export',. 'gq
-00000120: 6c61 6c63 6865 6d79 2e74 7261 6e73 666f  lalchemy.transfo
-00000130: 726d 6174 696f 6e73 2e69 6d70 6f72 7469  rmations.importi
-00000140: 6e67 272c 0a20 2767 716c 616c 6368 656d  ng',. 'gqlalchem
-00000150: 792e 7472 616e 7366 6f72 6d61 7469 6f6e  y.transformation
-00000160: 732e 7472 616e 736c 6174 6f72 7327 2c0a  s.translators',.
-00000170: 2027 6771 6c61 6c63 6865 6d79 2e76 656e   'gqlalchemy.ven
-00000180: 646f 7273 275d 0a0a 7061 636b 6167 655f  dors']..package_
-00000190: 6461 7461 203d 205c 0a7b 2727 3a20 5b27  data = \.{'': ['
-000001a0: 2a27 5d7d 0a0a 696e 7374 616c 6c5f 7265  *']}..install_re
-000001b0: 7175 6972 6573 203d 205c 0a5b 2761 646c  quires = \.['adl
-000001c0: 6673 3e3d 3230 3232 2e32 2e30 2c3c 3230  fs>=2022.2.0,<20
-000001d0: 3233 2e30 2e30 272c 0a20 2764 6163 6974  23.0.0',. 'dacit
-000001e0: 653e 3d31 2e36 2e30 2c3c 322e 302e 3027  e>=1.6.0,<2.0.0'
-000001f0: 2c0a 2027 6467 6c3e 3d30 2e39 2e31 2c3c  ,. 'dgl>=0.9.1,<
-00000200: 302e 3130 2e30 272c 0a20 2764 6f63 6b65  0.10.0',. 'docke
-00000210: 723e 3d35 2e30 2e33 2c3c 362e 302e 3027  r>=5.0.3,<6.0.0'
-00000220: 2c0a 2027 6e65 6f34 6a3e 3d34 2e34 2e33  ,. 'neo4j>=4.4.3
-00000230: 2c3c 352e 302e 3027 2c0a 2027 6e65 7477  ,<5.0.0',. 'netw
-00000240: 6f72 6b78 3e3d 322e 352e 312c 3c33 2e30  orkx>=2.5.1,<3.0
-00000250: 2e30 272c 0a20 276e 756d 7079 3e3d 312e  .0',. 'numpy>=1.
-00000260: 3234 2e31 2c3c 322e 302e 3027 2c0a 2027  24.1,<2.0.0',. '
-00000270: 7073 7574 696c 3e3d 352e 392e 302c 3c36  psutil>=5.9.0,<6
-00000280: 2e30 2e30 272c 0a20 2770 7961 7272 6f77  .0.0',. 'pyarrow
-00000290: 3e3d 392e 302e 302c 3c31 302e 302e 3027  >=9.0.0,<10.0.0'
-000002a0: 2c0a 2027 7079 6461 6e74 6963 3e3d 312e  ,. 'pydantic>=1.
-000002b0: 382e 322c 3c32 2e30 2e30 272c 0a20 2770  8.2,<2.0.0',. 'p
-000002c0: 796d 6763 6c69 656e 743d 3d31 2e33 2e31  ymgclient==1.3.1
-000002d0: 272c 0a20 2774 6f72 6368 3e3d 312e 3133  ',. 'torch>=1.13
-000002e0: 2e31 2c3c 322e 302e 3027 5d0a 0a73 6574  .1,<2.0.0']..set
-000002f0: 7570 5f6b 7761 7267 7320 3d20 7b0a 2020  up_kwargs = {.  
-00000300: 2020 276e 616d 6527 3a20 2767 716c 616c    'name': 'gqlal
-00000310: 6368 656d 7927 2c0a 2020 2020 2776 6572  chemy',.    'ver
-00000320: 7369 6f6e 273a 2027 312e 342e 3027 2c0a  sion': '1.4.0',.
-00000330: 2020 2020 2764 6573 6372 6970 7469 6f6e      'description
-00000340: 273a 2027 4751 4c41 6c63 6865 6d79 2069  ': 'GQLAlchemy i
-00000350: 7320 6c69 6272 6172 7920 6465 7665 6c6f  s library develo
-00000360: 7065 6420 7769 7468 2070 7572 706f 7365  ped with purpose
-00000370: 206f 6620 6173 7369 7374 696e 6720 7772   of assisting wr
-00000380: 6974 696e 6720 616e 6420 7275 6e6e 696e  iting and runnin
-00000390: 6720 7175 6572 6965 7320 6f6e 204d 656d  g queries on Mem
-000003a0: 6772 6170 682e 272c 0a20 2020 2027 6c6f  graph.',.    'lo
-000003b0: 6e67 5f64 6573 6372 6970 7469 6f6e 273a  ng_description':
-000003c0: 2027 2320 4751 4c41 6c63 6865 6d79 5c6e   '# GQLAlchemy\n
-000003d0: 5c6e 5c6e 3c70 3e5c 6e20 2020 203c 6120  \n\n<p>\n    <a 
-000003e0: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-000003f0: 7468 7562 2e63 6f6d 2f6d 656d 6772 6170  thub.com/memgrap
-00000400: 682f 6771 6c61 6c63 6865 6d79 2f61 6374  h/gqlalchemy/act
-00000410: 696f 6e73 223e 3c69 6d67 2073 7263 3d22  ions"><img src="
-00000420: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000430: 6f6d 2f6d 656d 6772 6170 682f 6771 6c61  om/memgraph/gqla
-00000440: 6c63 6865 6d79 2f77 6f72 6b66 6c6f 7773  lchemy/workflows
-00000450: 2f42 7569 6c64 2532 3061 6e64 2532 3054  /Build%20and%20T
-00000460: 6573 742f 6261 6467 652e 7376 6722 202f  est/badge.svg" /
-00000470: 3e3c 2f61 3e5c 6e20 2020 203c 6120 6872  ></a>\n    <a hr
-00000480: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
-00000490: 7562 2e63 6f6d 2f6d 656d 6772 6170 682f  ub.com/memgraph/
-000004a0: 6771 6c61 6c63 6865 6d79 2f62 6c6f 622f  gqlalchemy/blob/
-000004b0: 6d61 696e 2f4c 4943 454e 5345 223e 3c69  main/LICENSE"><i
-000004c0: 6d67 2073 7263 3d22 6874 7470 733a 2f2f  mg src="https://
-000004d0: 696d 672e 7368 6965 6c64 732e 696f 2f67  img.shields.io/g
-000004e0: 6974 6875 622f 6c69 6365 6e73 652f 6d65  ithub/license/me
-000004f0: 6d67 7261 7068 2f67 716c 616c 6368 656d  mgraph/gqlalchem
-00000500: 7922 202f 3e3c 2f61 3e5c 6e20 2020 203c  y" /></a>\n    <
-00000510: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
-00000520: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
-00000530: 2f67 716c 616c 6368 656d 7922 3e3c 696d  /gqlalchemy"><im
-00000540: 6720 7372 633d 2268 7474 7073 3a2f 2f69  g src="https://i
-00000550: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
-00000560: 7069 2f76 2f67 716c 616c 6368 656d 7922  pi/v/gqlalchemy"
-00000570: 202f 3e3c 2f61 3e5c 6e20 2020 203c 6120   /></a>\n    <a 
-00000580: 6872 6566 3d22 6874 7470 733a 2f2f 6769  href="https://gi
-00000590: 7468 7562 2e63 6f6d 2f70 7366 2f62 6c61  thub.com/psf/bla
-000005a0: 636b 223e 3c69 6d67 2061 6c74 3d22 436f  ck"><img alt="Co
-000005b0: 6465 2073 7479 6c65 3a20 626c 6163 6b22  de style: black"
-000005c0: 2073 7263 3d22 6874 7470 733a 2f2f 696d   src="https://im
-000005d0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000005e0: 6765 2f63 6f64 6525 3230 7374 796c 652d  ge/code%20style-
-000005f0: 626c 6163 6b2d 3030 3030 3030 2e73 7667  black-000000.svg
-00000600: 223e 3c2f 613e 5c6e 2020 2020 3c61 2068  "></a>\n    <a h
-00000610: 7265 663d 2268 7474 7073 3a2f 2f6d 656d  ref="https://mem
-00000620: 6772 6170 682e 636f 6d2f 646f 6373 2f67  graph.com/docs/g
-00000630: 716c 616c 6368 656d 7922 2061 6c74 3d22  qlalchemy" alt="
-00000640: 446f 6375 6d65 6e74 6174 696f 6e22 3e3c  Documentation"><
-00000650: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
-00000660: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000670: 6261 6467 652f 646f 6375 6d65 6e74 6174  badge/documentat
-00000680: 696f 6e2d 4751 4c41 6c63 6865 6d79 2d6f  ion-GQLAlchemy-o
-00000690: 7261 6e67 6522 202f 3e3c 2f61 3e5c 6e20  range" /></a>\n 
-000006a0: 2020 203c 6120 6872 6566 3d22 6874 7470     <a href="http
-000006b0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-000006c0: 656d 6772 6170 682f 6771 6c61 6c63 6865  emgraph/gqlalche
-000006d0: 6d79 2f73 7461 7267 617a 6572 7322 2061  my/stargazers" a
-000006e0: 6c74 3d22 5374 6172 6761 7a65 7273 223e  lt="Stargazers">
-000006f0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
-00000700: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
-00000710: 2f67 6974 6875 622f 7374 6172 732f 6d65  /github/stars/me
-00000720: 6d67 7261 7068 2f67 716c 616c 6368 656d  mgraph/gqlalchem
-00000730: 793f 7374 796c 653d 736f 6369 616c 2220  y?style=social" 
-00000740: 2f3e 3c2f 613e 5c6e 3c2f 703e 5c6e 5c6e  /></a>\n</p>\n\n
-00000750: 2a2a 4751 4c41 6c63 6865 6d79 2a2a 2069  **GQLAlchemy** i
-00000760: 7320 6120 6675 6c6c 7920 6f70 656e 2d73  s a fully open-s
-00000770: 6f75 7263 6520 5079 7468 6f6e 206c 6962  ource Python lib
-00000780: 7261 7279 2061 6e64 202a 2a4f 626a 6563  rary and **Objec
-00000790: 7420 4772 6170 6820 4d61 7070 6572 2a2a  t Graph Mapper**
-000007a0: 2028 4f47 4d29 202d 2061 206c 696e 6b20   (OGM) - a link 
-000007b0: 6265 7477 6565 6e20 6772 6170 6820 6461  between graph da
-000007c0: 7461 6261 7365 206f 626a 6563 7473 2061  tabase objects a
-000007d0: 6e64 2050 7974 686f 6e20 6f62 6a65 6374  nd Python object
-000007e0: 732e 5c6e 5c6e 416e 204f 626a 6563 7420  s.\n\nAn Object 
-000007f0: 4772 6170 6820 4d61 7070 6572 206f 7220  Graph Mapper or 
-00000800: 4f47 4d20 7072 6f76 6964 6573 2061 2064  OGM provides a d
-00000810: 6576 656c 6f70 6572 2d66 7269 656e 646c  eveloper-friendl
-00000820: 7920 776f 726b 666c 6f77 2074 6861 7420  y workflow that 
-00000830: 616c 6c6f 7773 2066 6f72 2077 7269 7469  allows for writi
-00000840: 6e67 206f 626a 6563 742d 6f72 6965 6e74  ng object-orient
-00000850: 6564 206e 6f74 6174 696f 6e20 746f 2063  ed notation to c
-00000860: 6f6d 6d75 6e69 6361 7465 2077 6974 6820  ommunicate with 
-00000870: 6772 6170 6820 6461 7461 6261 7365 732e  graph databases.
-00000880: 2049 6e73 7465 6164 206f 6620 7772 6974   Instead of writ
-00000890: 696e 6720 4379 7068 6572 2071 7565 7269  ing Cypher queri
-000008a0: 6573 2c20 796f 7520 7769 6c6c 2062 6520  es, you will be 
-000008b0: 6162 6c65 2074 6f20 7772 6974 6520 6f62  able to write ob
-000008c0: 6a65 6374 2d6f 7269 656e 7465 6420 636f  ject-oriented co
-000008d0: 6465 2c20 7768 6963 6820 7468 6520 4f47  de, which the OG
-000008e0: 4d20 7769 6c6c 2061 7574 6f6d 6174 6963  M will automatic
-000008f0: 616c 6c79 2074 7261 6e73 6c61 7465 2069  ally translate i
-00000900: 6e74 6f20 4379 7068 6572 2071 7565 7269  nto Cypher queri
-00000910: 6573 2e5c 6e5c 6e47 514c 416c 6368 656d  es.\n\nGQLAlchem
-00000920: 7920 6973 2062 7569 6c74 206f 6e20 746f  y is built on to
-00000930: 7020 6f66 204d 656d 6772 6170 685c 2773  p of Memgraph\'s
-00000940: 206c 6f77 2d6c 6576 656c 2050 7974 686f   low-level Pytho
-00000950: 6e20 636c 6965 6e74 2060 7079 6d67 636c  n client `pymgcl
-00000960: 6965 6e74 605c 6e28 5b50 7950 495d 2868  ient`\n([PyPI](h
-00000970: 7474 7073 3a2f 2f70 7970 692e 6f72 672f  ttps://pypi.org/
-00000980: 7072 6f6a 6563 742f 7079 6d67 636c 6965  project/pymgclie
-00000990: 6e74 2f29 202f 5c6e 5b44 6f63 756d 656e  nt/) /\n[Documen
-000009a0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
-000009b0: 6d65 6d67 7261 7068 2e67 6974 6875 622e  memgraph.github.
-000009c0: 696f 2f70 796d 6763 6c69 656e 742f 2920  io/pymgclient/) 
-000009d0: 2f5c 6e5b 4769 7448 7562 5d28 6874 7470  /\n[GitHub](http
-000009e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6d  s://github.com/m
-000009f0: 656d 6772 6170 682f 7079 6d67 636c 6965  emgraph/pymgclie
-00000a00: 6e74 2929 2e5c 6e5c 6e23 2320 496e 7374  nt)).\n\n## Inst
-00000a10: 616c 6c61 7469 6f6e 5c6e 5c6e 4265 666f  allation\n\nBefo
-00000a20: 7265 2079 6f75 2069 6e73 7461 6c6c 2060  re you install `
-00000a30: 6771 6c61 6c63 6865 6d79 602c 206d 616b  gqlalchemy`, mak
-00000a40: 6520 7375 7265 2074 6861 7420 796f 7520  e sure that you 
-00000a50: 6861 7665 2060 636d 616b 6560 2069 6e73  have `cmake` ins
-00000a60: 7461 6c6c 6564 2062 7920 7275 6e6e 696e  talled by runnin
-00000a70: 673a 5c6e 6060 605c 6e63 6d61 6b65 202d  g:\n```\ncmake -
-00000a80: 2d76 6572 7369 6f6e 5c6e 6060 605c 6e59  -version\n```\nY
-00000a90: 6f75 2063 616e 2069 6e73 7461 6c6c 2060  ou can install `
-00000aa0: 636d 616b 6560 2062 7920 666f 6c6c 6f77  cmake` by follow
-00000ab0: 696e 6720 7468 6520 5b6f 6666 6963 6961  ing the [officia
-00000ac0: 6c20 696e 7374 7275 6374 696f 6e73 5d28  l instructions](
-00000ad0: 6874 7470 733a 2f2f 6367 6f6c 642e 7265  https://cgold.re
-00000ae0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-00000af0: 6c61 7465 7374 2f66 6972 7374 2d73 7465  latest/first-ste
-00000b00: 702f 696e 7374 616c 6c61 7469 6f6e 2e68  p/installation.h
-00000b10: 746d 6c23 292e 5c6e 5c6e 546f 2069 6e73  tml#).\n\nTo ins
-00000b20: 7461 6c6c 2060 6771 6c61 6c63 6865 6d79  tall `gqlalchemy
-00000b30: 602c 2073 696d 706c 7920 7275 6e20 7468  `, simply run th
-00000b40: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
-00000b50: 616e 643a 5c6e 6060 605c 6e70 6970 2069  and:\n```\npip i
-00000b60: 6e73 7461 6c6c 2067 716c 616c 6368 656d  nstall gqlalchem
-00000b70: 795c 6e60 6060 5c6e 5c6e 4966 2079 6f75  y\n```\n\nIf you
-00000b80: 2061 7265 2075 7369 6e67 205b 436f 6e64   are using [Cond
-00000b90: 615d 2868 7474 7073 3a2f 2f64 6f63 732e  a](https://docs.
-00000ba0: 636f 6e64 612e 696f 2f65 6e2f 6c61 7465  conda.io/en/late
-00000bb0: 7374 2f29 2066 6f72 2050 7974 686f 6e20  st/) for Python 
-00000bc0: 656e 7669 726f 6e6d 656e 7420 6d61 6e61  environment mana
-00000bd0: 6765 6d65 6e74 2c20 796f 7520 6361 6e20  gement, you can 
-00000be0: 696e 7374 616c 6c20 4751 4c41 6c63 6865  install GQLAlche
-00000bf0: 6d79 2074 6872 6f75 6768 2070 6970 2e5c  my through pip.\
-00000c00: 6e5c 6e23 2320 4275 696c 6420 2620 5465  n\n## Build & Te
-00000c10: 7374 5c6e 5c6e 5468 6520 7072 6f6a 6563  st\n\nThe projec
-00000c20: 7420 7573 6573 205b 506f 6574 7279 5d28  t uses [Poetry](
-00000c30: 6874 7470 733a 2f2f 7079 7468 6f6e 2d70  https://python-p
-00000c40: 6f65 7472 792e 6f72 672f 2920 746f 2062  oetry.org/) to b
-00000c50: 7569 6c64 2074 6865 2047 514c 416c 6368  uild the GQLAlch
-00000c60: 656d 7920 5079 7468 6f6e 206c 6962 7261  emy Python libra
-00000c70: 7279 2e20 546f 2062 7569 6c64 2061 6e64  ry. To build and
-00000c80: 2072 756e 2074 6573 7473 2c20 6578 6563   run tests, exec
-00000c90: 7574 6520 7468 6520 666f 6c6c 6f77 696e  ute the followin
-00000ca0: 6720 636f 6d6d 616e 643a 5c6e 6070 6f65  g command:\n`poe
-00000cb0: 7472 7920 696e 7374 616c 6c60 5c6e 5c6e  try install`\n\n
-00000cc0: 4265 666f 7265 2073 7461 7274 696e 6720  Before starting 
-00000cd0: 7468 6520 7465 7374 732c 206d 616b 6520  the tests, make 
-00000ce0: 7375 7265 2079 6f75 2068 6176 6520 616e  sure you have an
-00000cf0: 2061 6374 6976 6520 4d65 6d67 7261 7068   active Memgraph
-00000d00: 2069 6e73 7461 6e63 6520 7275 6e6e 696e   instance runnin
-00000d10: 672e 2045 7865 6375 7465 2074 6865 2066  g. Execute the f
-00000d20: 6f6c 6c6f 7769 6e67 2063 6f6d 6d61 6e64  ollowing command
-00000d30: 3a5c 6e60 706f 6574 7279 2072 756e 2070  :\n`poetry run p
-00000d40: 7974 6573 7420 2e60 5c6e 5c6e 2323 2047  ytest .`\n\n## G
-00000d50: 514c 416c 6368 656d 7920 6361 7061 6269  QLAlchemy capabi
-00000d60: 6c69 7469 6573 5c6e 5c6e 3c64 6574 6169  lities\n\n<detai
-00000d70: 6c73 3e5c 6e3c 7375 6d6d 6172 793e f09f  ls>\n<summary>..
-00000d80: 97ba efb8 8f20 4f62 6a65 6374 2067 7261  ..... Object gra
-00000d90: 7068 206d 6170 7065 723c 2f73 756d 6d61  ph mapper</summa
-00000da0: 7279 3e5c 6e3c 6272 3e5c 6e5c 6e42 656c  ry>\n<br>\n\nBel
-00000db0: 6f77 2079 6f75 2063 616e 2073 6565 2061  ow you can see a
-00000dc0: 6e20 6578 616d 706c 6520 6f66 2068 6f77  n example of how
-00000dd0: 2074 6f20 6372 6561 7465 2060 5573 6572   to create `User
-00000de0: 6020 616e 6420 604c 616e 6775 6167 6560  ` and `Language`
-00000df0: 206e 6f64 6520 636c 6173 7365 732c 2061   node classes, a
-00000e00: 6e64 2061 2072 656c 6174 696f 6e73 6869  nd a relationshi
-00000e10: 7020 636c 6173 7320 6f66 2074 7970 6520  p class of type 
-00000e20: 6053 5045 414b 5360 2e20 416c 6f6e 6720  `SPEAKS`. Along 
-00000e30: 7769 7468 2074 6861 742c 2079 6f75 2063  with that, you c
-00000e40: 616e 2073 6565 2068 6f77 2074 6f20 6372  an see how to cr
-00000e50: 6561 7465 2061 206e 6577 206e 6f64 6520  eate a new node 
-00000e60: 616e 6420 7265 6c61 7469 6f6e 7368 6970  and relationship
-00000e70: 2061 6e64 2068 6f77 2074 6f20 7361 7665   and how to save
-00000e80: 2074 6865 6d20 696e 2074 6865 2064 6174   them in the dat
-00000e90: 6162 6173 652e 2041 6674 6572 2074 6861  abase. After tha
-00000ea0: 742c 2079 6f75 2063 616e 206c 6f61 6420  t, you can load 
-00000eb0: 7468 6f73 6520 6e6f 6465 7320 616e 6420  those nodes and 
-00000ec0: 7265 6c61 7469 6f6e 7368 6970 2066 726f  relationship fro
-00000ed0: 6d20 7468 6520 6461 7461 6261 7365 2e5c  m the database.\
-00000ee0: 6e3c 6272 3e5c 6e3c 6272 3e5c 6e5c 6e60  n<br>\n<br>\n\n`
-00000ef0: 6060 7079 7468 6f6e 5c6e 6672 6f6d 2067  ``python\nfrom g
-00000f00: 716c 616c 6368 656d 7920 696d 706f 7274  qlalchemy import
-00000f10: 204d 656d 6772 6170 682c 204e 6f64 652c   Memgraph, Node,
-00000f20: 2052 656c 6174 696f 6e73 6869 702c 2046   Relationship, F
-00000f30: 6965 6c64 5c6e 6672 6f6d 2074 7970 696e  ield\nfrom typin
-00000f40: 6720 696d 706f 7274 204f 7074 696f 6e61  g import Optiona
-00000f50: 6c5c 6e5c 6e64 6220 3d20 4d65 6d67 7261  l\n\ndb = Memgra
-00000f60: 7068 2829 5c6e 5c6e 636c 6173 7320 5573  ph()\n\nclass Us
-00000f70: 6572 284e 6f64 652c 2069 6e64 6578 3d54  er(Node, index=T
-00000f80: 7275 652c 2064 623d 6462 293a 5c6e 2020  rue, db=db):\n  
-00000f90: 2020 6964 3a20 7374 7220 3d20 4669 656c    id: str = Fiel
-00000fa0: 6428 696e 6465 783d 5472 7565 2c20 6578  d(index=True, ex
-00000fb0: 6973 743d 5472 7565 2c20 756e 6971 7565  ist=True, unique
-00000fc0: 3d54 7275 652c 2064 623d 6462 295c 6e5c  =True, db=db)\n\
-00000fd0: 6e63 6c61 7373 204c 616e 6775 6167 6528  nclass Language(
-00000fe0: 4e6f 6465 293a 5c6e 2020 2020 6e61 6d65  Node):\n    name
-00000ff0: 3a20 7374 7220 3d20 4669 656c 6428 756e  : str = Field(un
-00001000: 6971 7565 3d54 7275 652c 2064 623d 6462  ique=True, db=db
-00001010: 295c 6e5c 6e63 6c61 7373 2053 7065 616b  )\n\nclass Speak
-00001020: 7328 5265 6c61 7469 6f6e 7368 6970 2c20  s(Relationship, 
-00001030: 7479 7065 3d22 5350 4541 4b53 2229 3a5c  type="SPEAKS"):\
-00001040: 6e20 2020 2070 6173 735c 6e5c 6e75 7365  n    pass\n\nuse
-00001050: 7220 3d20 5573 6572 2869 643d 2233 222c  r = User(id="3",
-00001060: 2075 7365 726e 616d 653d 224a 6f68 6e22   username="John"
-00001070: 292e 7361 7665 2864 6229 5c6e 6c61 6e67  ).save(db)\nlang
-00001080: 7561 6765 203d 204c 616e 6775 6167 6528  uage = Language(
-00001090: 6e61 6d65 3d22 656e 2229 2e73 6176 6528  name="en").save(
-000010a0: 6462 295c 6e73 7065 616b 735f 7265 6c20  db)\nspeaks_rel 
-000010b0: 3d20 5370 6561 6b73 285c 6e20 2020 205f  = Speaks(\n    _
-000010c0: 7374 6172 745f 6e6f 6465 5f69 6420 3d20  start_node_id = 
-000010d0: 7573 6572 2e5f 6964 2c5c 6e20 2020 205f  user._id,\n    _
-000010e0: 656e 645f 6e6f 6465 5f69 6420 3d20 6c61  end_node_id = la
-000010f0: 6e67 7561 6765 2e5f 6964 5c6e 292e 7361  nguage._id\n).sa
-00001100: 7665 2864 6229 5c6e 5c6e 6c6f 6164 6564  ve(db)\n\nloaded
-00001110: 5f75 7365 7220 3d20 5573 6572 2869 643d  _user = User(id=
-00001120: 2233 2229 2e6c 6f61 6428 6462 3d64 6229  "3").load(db=db)
-00001130: 5c6e 7072 696e 7428 6c6f 6164 6564 5f75  \nprint(loaded_u
-00001140: 7365 7229 5c6e 6c6f 6164 6564 5f73 7065  ser)\nloaded_spe
-00001150: 616b 7320 3d20 5370 6561 6b73 285c 6e20  aks = Speaks(\n 
-00001160: 2020 2020 2020 205f 7374 6172 745f 6e6f         _start_no
-00001170: 6465 5f69 643d 7573 6572 2e5f 6964 2c5c  de_id=user._id,\
-00001180: 6e20 2020 2020 2020 205f 656e 645f 6e6f  n        _end_no
-00001190: 6465 5f69 643d 6c61 6e67 7561 6765 2e5f  de_id=language._
-000011a0: 6964 5c6e 2020 2020 292e 6c6f 6164 2864  id\n    ).load(d
-000011b0: 6229 5c6e 7072 696e 7428 6c6f 6164 6564  b)\nprint(loaded
-000011c0: 5f73 7065 616b 7329 5c6e 6060 605c 6e3c  _speaks)\n```\n<
-000011d0: 2f64 6574 6169 6c73 3e5c 6e5c 6e3c 6465  /details>\n\n<de
-000011e0: 7461 696c 733e 5c6e 3c73 756d 6d61 7279  tails>\n<summary
-000011f0: 3ef0 9f94 a820 5175 6572 7920 6275 696c  >.... Query buil
-00001200: 6465 723c 2f73 756d 6d61 7279 3e5c 6e3c  der</summary>\n<
-00001210: 6272 3e5c 6e57 6865 6e20 6275 696c 6469  br>\nWhen buildi
-00001220: 6e67 2061 2043 7970 6865 7220 7175 6572  ng a Cypher quer
-00001230: 792c 2079 6f75 2063 616e 2075 7365 2061  y, you can use a
-00001240: 2073 6574 206f 6620 6d65 7468 6f64 7320   set of methods 
-00001250: 7468 6174 2061 7265 2077 7261 7070 6572  that are wrapper
-00001260: 7320 6172 6f75 6e64 2043 7970 6865 7220  s around Cypher 
-00001270: 636c 6175 7365 732e 205c 6e3c 6272 3e5c  clauses. \n<br>\
-00001280: 6e3c 6272 3e5c 6e5c 6e60 6060 7079 7468  n<br>\n\n```pyth
-00001290: 6f6e 5c6e 6672 6f6d 2067 716c 616c 6368  on\nfrom gqlalch
-000012a0: 656d 7920 696d 706f 7274 2063 7265 6174  emy import creat
-000012b0: 652c 206d 6174 6368 5c6e 6672 6f6d 2067  e, match\nfrom g
-000012c0: 716c 616c 6368 656d 792e 7175 6572 795f  qlalchemy.query_
-000012d0: 6275 696c 6465 7220 696d 706f 7274 204f  builder import O
-000012e0: 7065 7261 746f 725c 6e5c 6e71 7565 7279  perator\n\nquery
-000012f0: 5f63 7265 6174 6520 3d20 6372 6561 7465  _create = create
-00001300: 2829 5c6e 2020 2020 2020 2020 2e6e 6f64  ()\n        .nod
-00001310: 6528 6c61 6265 6c73 3d22 5065 7273 6f6e  e(labels="Person
-00001320: 222c 206e 616d 653d 224c 6573 6c69 6522  ", name="Leslie"
-00001330: 295c 6e20 2020 2020 2020 202e 746f 2872  )\n        .to(r
-00001340: 656c 6174 696f 6e73 6869 705f 7479 7065  elationship_type
-00001350: 3d22 4652 4945 4e44 535f 5749 5448 2229  ="FRIENDS_WITH")
-00001360: 5c6e 2020 2020 2020 2020 2e6e 6f64 6528  \n        .node(
-00001370: 6c61 6265 6c73 3d22 5065 7273 6f6e 222c  labels="Person",
-00001380: 206e 616d 653d 2252 6f6e 2229 5c6e 2020   name="Ron")\n  
-00001390: 2020 2020 2020 2e65 7865 6375 7465 2829        .execute()
-000013a0: 5c6e 5c6e 7175 6572 795f 6d61 7463 6820  \n\nquery_match 
-000013b0: 3d20 6d61 7463 6828 295c 6e20 2020 2020  = match()\n     
-000013c0: 2020 202e 6e6f 6465 286c 6162 656c 733d     .node(labels=
-000013d0: 2250 6572 736f 6e22 2c20 7661 7269 6162  "Person", variab
-000013e0: 6c65 3d22 7031 2229 5c6e 2020 2020 2020  le="p1")\n      
-000013f0: 2020 2e74 6f28 295c 6e20 2020 2020 2020    .to()\n       
-00001400: 202e 6e6f 6465 286c 6162 656c 733d 2250   .node(labels="P
-00001410: 6572 736f 6e22 2c20 7661 7269 6162 6c65  erson", variable
-00001420: 3d22 7032 2229 5c6e 2020 2020 2020 2020  ="p2")\n        
-00001430: 2e77 6865 7265 2869 7465 6d3d 2270 312e  .where(item="p1.
-00001440: 6e61 6d65 222c 206f 7065 7261 746f 723d  name", operator=
-00001450: 4f70 6572 6174 6f72 2e45 5155 414c 2c20  Operator.EQUAL, 
-00001460: 6c69 7465 7261 6c3d 224c 6573 6c69 6522  literal="Leslie"
-00001470: 295c 6e20 2020 2020 2020 202e 7265 7475  )\n        .retu
-00001480: 726e 5f28 7265 7375 6c74 733d 5b22 7031  rn_(results=["p1
-00001490: 222c 2028 2270 3222 2c20 2273 6563 6f6e  ", ("p2", "secon
-000014a0: 6422 295d 295c 6e20 2020 2020 2020 202e  d")])\n        .
-000014b0: 6578 6563 7574 6528 295c 6e60 6060 5c6e  execute()\n```\n
-000014c0: 3c2f 6465 7461 696c 733e 5c6e 5c6e 3c64  </details>\n\n<d
-000014d0: 6574 6169 6c73 3e5c 6e3c 7375 6d6d 6172  etails>\n<summar
-000014e0: 793e f09f 9ab0 204d 616e 6167 6520 7374  y>.... Manage st
-000014f0: 7265 616d 733c 2f73 756d 6d61 7279 3e5c  reams</summary>\
-00001500: 6e3c 6272 3e5c 6e5c 6e59 6f75 2063 616e  n<br>\n\nYou can
-00001510: 2063 7265 6174 6520 616e 6420 7374 6172   create and star
-00001520: 7420 4b61 666b 6120 6f72 2050 756c 7361  t Kafka or Pulsa
-00001530: 7220 7374 7265 616d 2075 7369 6e67 2047  r stream using G
-00001540: 514c 416c 6368 656d 792e 205c 6e3c 6272  QLAlchemy. \n<br
-00001550: 3e5c 6e5c 6e2a 2a4b 6166 6b61 2073 7472  >\n\n**Kafka str
-00001560: 6561 6d2a 2a20 5c6e 6060 6070 7974 686f  eam** \n```pytho
-00001570: 6e5c 6e66 726f 6d20 6771 6c61 6c63 6865  n\nfrom gqlalche
-00001580: 6d79 2069 6d70 6f72 7420 4d65 6d67 7261  my import Memgra
-00001590: 7068 4b61 666b 6153 7472 6561 6d5c 6e5c  phKafkaStream\n\
-000015a0: 6e73 7472 6561 6d20 3d20 4d65 6d67 7261  nstream = Memgra
-000015b0: 7068 4b61 666b 6153 7472 6561 6d28 6e61  phKafkaStream(na
-000015c0: 6d65 3d22 7261 7469 6e67 735f 7374 7265  me="ratings_stre
-000015d0: 616d 222c 2074 6f70 6963 733d 5b22 7261  am", topics=["ra
-000015e0: 7469 6e67 7322 5d2c 2074 7261 6e73 666f  tings"], transfo
-000015f0: 726d 3d22 6d6f 7669 656c 656e 732e 7261  rm="movielens.ra
-00001600: 7469 6e67 222c 2062 6f6f 7473 7472 6170  ting", bootstrap
-00001610: 5f73 6572 7665 7273 3d22 6c6f 6361 6c68  _servers="localh
-00001620: 6f73 743a 3930 3933 2229 5c6e 6462 2e63  ost:9093")\ndb.c
-00001630: 7265 6174 655f 7374 7265 616d 2873 7472  reate_stream(str
-00001640: 6561 6d29 5c6e 6462 2e73 7461 7274 5f73  eam)\ndb.start_s
-00001650: 7472 6561 6d28 7374 7265 616d 295c 6e60  tream(stream)\n`
-00001660: 6060 5c6e 5c6e 5c6e 2a2a 5075 6c73 6172  ``\n\n\n**Pulsar
-00001670: 2073 7472 6561 6d2a 2a5c 6e60 6060 7079   stream**\n```py
-00001680: 7468 6f6e 5c6e 6672 6f6d 2067 716c 616c  thon\nfrom gqlal
-00001690: 6368 656d 7920 696d 706f 7274 204d 656d  chemy import Mem
-000016a0: 6772 6170 6850 756c 7361 7253 7472 6561  graphPulsarStrea
-000016b0: 6d5c 6e5c 6e73 7472 6561 6d20 3d20 4d65  m\n\nstream = Me
-000016c0: 6d67 7261 7068 5075 6c73 6172 5374 7265  mgraphPulsarStre
-000016d0: 616d 286e 616d 653d 2272 6174 696e 6773  am(name="ratings
-000016e0: 5f73 7472 6561 6d22 2c20 746f 7069 6373  _stream", topics
-000016f0: 3d5b 2272 6174 696e 6773 225d 2c20 7472  =["ratings"], tr
-00001700: 616e 7366 6f72 6d3d 226d 6f76 6965 6c65  ansform="moviele
-00001710: 6e73 2e72 6174 696e 6722 2c20 7365 7276  ns.rating", serv
-00001720: 6963 655f 7572 6c3d 226c 6f63 616c 686f  ice_url="localho
-00001730: 7374 3a36 3635 3022 295c 6e64 622e 6372  st:6650")\ndb.cr
-00001740: 6561 7465 5f73 7472 6561 6d28 7374 7265  eate_stream(stre
-00001750: 616d 295c 6e64 622e 7374 6172 745f 7374  am)\ndb.start_st
-00001760: 7265 616d 2873 7472 6561 6d29 5c6e 6060  ream(stream)\n``
-00001770: 605c 6e5c 6e3c 2f64 6574 6169 6c73 3e5c  `\n\n</details>\
-00001780: 6e5c 6e3c 6465 7461 696c 733e 5c6e 3c73  n\n<details>\n<s
-00001790: 756d 6d61 7279 3ef0 9f97 84ef b88f 2049  ummary>....... I
-000017a0: 6d70 6f72 7420 7461 626c 6520 6461 7461  mport table data
-000017b0: 2066 726f 6d20 6469 6666 6572 656e 7420   from different 
-000017c0: 736f 7572 6365 733c 2f73 756d 6d61 7279  sources</summary
-000017d0: 3e5c 6e3c 6272 3e5c 6e5c 6e2a 2a49 6d70  >\n<br>\n\n**Imp
-000017e0: 6f72 7420 7461 626c 6520 6461 7461 2074  ort table data t
-000017f0: 6f20 6120 6772 6170 6820 6461 7461 6261  o a graph databa
-00001800: 7365 2a2a 5c6e 5c6e 596f 7520 6361 6e20  se**\n\nYou can 
-00001810: 7472 616e 736c 6174 6520 7461 626c 6520  translate table 
-00001820: 6461 7461 2066 726f 6d20 6120 6669 6c65  data from a file
-00001830: 2074 6f20 6772 6170 6820 6461 7461 2061   to graph data a
-00001840: 6e64 2069 6d70 6f72 7420 6974 2074 6f20  nd import it to 
-00001850: 4d65 6d67 7261 7068 2e20 4375 7272 656e  Memgraph. Curren
-00001860: 746c 792c 2077 6520 7375 7070 6f72 7420  tly, we support 
-00001870: 7265 6164 696e 6720 6f66 2043 5356 2c20  reading of CSV, 
-00001880: 5061 7271 7565 742c 204f 5243 2061 6e64  Parquet, ORC and
-00001890: 2049 5043 2f46 6561 7468 6572 2f41 7272   IPC/Feather/Arr
-000018a0: 6f77 2066 696c 6520 666f 726d 6174 7320  ow file formats 
-000018b0: 7669 6120 7468 6520 5079 4172 726f 7720  via the PyArrow 
-000018c0: 7061 636b 6167 652e 5c6e 5c6e 5265 6164  package.\n\nRead
-000018d0: 2061 6c6c 2061 626f 7574 2069 7420 696e   all about it in
-000018e0: 205b 7461 626c 6520 746f 2067 7261 7068   [table to graph
-000018f0: 2069 6d70 6f72 7465 7220 686f 772d 746f   importer how-to
-00001900: 2067 7569 6465 5d28 6874 7470 733a 2f2f   guide](https://
-00001910: 6d65 6d67 7261 7068 2e63 6f6d 2f64 6f63  memgraph.com/doc
-00001920: 732f 6771 6c61 6c63 6865 6d79 2f68 6f77  s/gqlalchemy/how
-00001930: 2d74 6f2d 6775 6964 6573 2f74 6162 6c65  -to-guides/table
-00001940: 2d74 6f2d 6772 6170 682d 696d 706f 7274  -to-graph-import
-00001950: 6572 292e 5c6e 5c6e 2a2a 4d61 6b65 2061  er).\n\n**Make a
-00001960: 2063 7573 746f 6d20 6669 6c65 2073 7973   custom file sys
-00001970: 7465 6d20 696d 706f 7274 6572 2a2a 5c6e  tem importer**\n
-00001980: 5c6e 4966 2079 6f75 2077 616e 7420 746f  \nIf you want to
-00001990: 2072 6561 6420 6672 6f6d 2061 2066 696c   read from a fil
-000019a0: 6520 7379 7374 656d 206e 6f74 2063 7572  e system not cur
-000019b0: 7265 6e74 6c79 2073 7570 706f 7274 6564  rently supported
-000019c0: 2062 7920 4751 4c41 6c63 6865 6d79 2c20   by GQLAlchemy, 
-000019d0: 6f72 2075 7365 2061 2066 696c 6520 7479  or use a file ty
-000019e0: 7065 2063 7572 7265 6e74 6c79 206e 6f74  pe currently not
-000019f0: 2072 6561 6461 626c 652c 2079 6f75 2063   readable, you c
-00001a00: 616e 2069 6d70 6c65 6d65 6e74 2079 6f75  an implement you
-00001a10: 7220 6f77 6e20 6279 2065 7874 656e 6469  r own by extendi
-00001a20: 6e67 2061 6273 7472 6163 7420 636c 6173  ng abstract clas
-00001a30: 7365 7320 6046 696c 6553 7973 7465 6d48  ses `FileSystemH
-00001a40: 616e 646c 6572 6020 616e 6420 6044 6174  andler` and `Dat
-00001a50: 614c 6f61 6465 7260 2c20 7265 7370 6563  aLoader`, respec
-00001a60: 7469 7665 6c79 2e5c 6e5c 6e52 6561 6420  tively.\n\nRead 
-00001a70: 616c 6c20 6162 6f75 7420 6974 2069 6e20  all about it in 
-00001a80: 5b63 7573 746f 6d20 6669 6c65 2073 7973  [custom file sys
-00001a90: 7465 6d20 696d 706f 7274 6572 2068 6f77  tem importer how
-00001aa0: 2d74 6f20 6775 6964 655d 2868 7474 7073  -to guide](https
-00001ab0: 3a2f 2f6d 656d 6772 6170 682e 636f 6d2f  ://memgraph.com/
-00001ac0: 646f 6373 2f67 716c 616c 6368 656d 792f  docs/gqlalchemy/
-00001ad0: 686f 772d 746f 2d67 7569 6465 732f 6375  how-to-guides/cu
-00001ae0: 7374 6f6d 2d66 696c 652d 7379 7374 656d  stom-file-system
-00001af0: 2d69 6d70 6f72 7465 7229 2e5c 6e5c 6e3c  -importer).\n\n<
-00001b00: 2f64 6574 6169 6c73 3e5c 6e5c 6e3c 6465  /details>\n\n<de
-00001b10: 7461 696c 733e 5c6e 3c73 756d 6d61 7279  tails>\n<summary
-00001b20: 3ee2 9a99 efb8 8f20 4d61 6e61 6765 204d  >...... Manage M
-00001b30: 656d 6772 6170 6820 696e 7374 616e 6365  emgraph instance
-00001b40: 733c 2f73 756d 6d61 7279 3e5c 6e3c 6272  s</summary>\n<br
-00001b50: 3e5c 6e5c 6e59 6f75 2063 616e 2073 7461  >\n\nYou can sta
-00001b60: 7274 2c20 7374 6f70 2c20 636f 6e6e 6563  rt, stop, connec
-00001b70: 7420 746f 2061 6e64 206d 6f6e 6974 6f72  t to and monitor
-00001b80: 204d 656d 6772 6170 6820 696e 7374 616e   Memgraph instan
-00001b90: 6365 7320 7769 7468 2047 514c 416c 6368  ces with GQLAlch
-00001ba0: 656d 792e 5c6e 5c6e 2a2a 4d61 6e61 6765  emy.\n\n**Manage
-00001bb0: 204d 656d 6772 6170 6820 446f 636b 6572   Memgraph Docker
-00001bc0: 2069 6e73 7461 6e63 652a 2a5c 6e5c 6e60   instance**\n\n`
-00001bd0: 6060 7079 7468 6f6e 5c6e 6672 6f6d 2067  ``python\nfrom g
-00001be0: 716c 616c 6368 656d 792e 696e 7374 616e  qlalchemy.instan
-00001bf0: 6365 5f72 756e 6e65 7220 696d 706f 7274  ce_runner import
-00001c00: 2028 5c6e 2020 2020 446f 636b 6572 496d   (\n    DockerIm
-00001c10: 6167 652c 5c6e 2020 2020 4d65 6d67 7261  age,\n    Memgra
-00001c20: 7068 496e 7374 616e 6365 446f 636b 6572  phInstanceDocker
-00001c30: 5c6e 295c 6e5c 6e6d 656d 6772 6170 685f  \n)\n\nmemgraph_
-00001c40: 696e 7374 616e 6365 203d 204d 656d 6772  instance = Memgr
-00001c50: 6170 6849 6e73 7461 6e63 6544 6f63 6b65  aphInstanceDocke
-00001c60: 7228 5c6e 2020 2020 646f 636b 6572 5f69  r(\n    docker_i
-00001c70: 6d61 6765 3d44 6f63 6b65 7249 6d61 6765  mage=DockerImage
-00001c80: 2e4d 454d 4752 4150 482c 2064 6f63 6b65  .MEMGRAPH, docke
-00001c90: 725f 696d 6167 655f 7461 673d 226c 6174  r_image_tag="lat
-00001ca0: 6573 7422 2c20 686f 7374 3d22 302e 302e  est", host="0.0.
-00001cb0: 302e 3022 2c20 706f 7274 3d37 3638 375c  0.0", port=7687\
-00001cc0: 6e29 5c6e 6d65 6d67 7261 7068 203d 206d  n)\nmemgraph = m
-00001cd0: 656d 6772 6170 685f 696e 7374 616e 6365  emgraph_instance
-00001ce0: 2e73 7461 7274 5f61 6e64 5f63 6f6e 6e65  .start_and_conne
-00001cf0: 6374 2872 6573 7461 7274 3d46 616c 7365  ct(restart=False
-00001d00: 295c 6e5c 6e6d 656d 6772 6170 682e 6578  )\n\nmemgraph.ex
-00001d10: 6563 7574 655f 616e 645f 6665 7463 6828  ecute_and_fetch(
-00001d20: 2252 4554 5552 4e20 5c27 4d65 6d67 7261  "RETURN \'Memgra
-00001d30: 7068 2069 7320 7275 6e6e 696e 675c 2720  ph is running\' 
-00001d40: 4153 2072 6573 756c 7422 2929 5b30 5d5b  AS result"))[0][
-00001d50: 2272 6573 756c 7422 5d5c 6e60 6060 5c6e  "result"]\n```\n
-00001d60: 5c6e 2a2a 4d61 6e61 6765 204d 656d 6772  \n**Manage Memgr
-00001d70: 6170 6820 6269 6e61 7279 2069 6e73 7461  aph binary insta
-00001d80: 6e63 652a 2a5c 6e5c 6e60 6060 7079 7468  nce**\n\n```pyth
-00001d90: 6f6e 5c6e 6672 6f6d 2067 716c 616c 6368  on\nfrom gqlalch
-00001da0: 656d 792e 696e 7374 616e 6365 5f72 756e  emy.instance_run
-00001db0: 6e65 7220 696d 706f 7274 204d 656d 6772  ner import Memgr
-00001dc0: 6170 6849 6e73 7461 6e63 6542 696e 6172  aphInstanceBinar
-00001dd0: 795c 6e5c 6e6d 656d 6772 6170 685f 696e  y\n\nmemgraph_in
-00001de0: 7374 616e 6365 203d 204d 656d 6772 6170  stance = Memgrap
-00001df0: 6849 6e73 7461 6e63 6542 696e 6172 7928  hInstanceBinary(
-00001e00: 5c6e 2020 2020 686f 7374 3d22 302e 302e  \n    host="0.0.
-00001e10: 302e 3022 2c20 706f 7274 3d37 3639 382c  0.0", port=7698,
-00001e20: 2062 696e 6172 795f 7061 7468 3d22 2f75   binary_path="/u
-00001e30: 7372 2f6c 6962 2f6d 656d 6772 6170 682f  sr/lib/memgraph/
-00001e40: 6d65 6d67 7261 7068 222c 2075 7365 723d  memgraph", user=
-00001e50: 226d 656d 6772 6170 6822 5c6e 295c 6e6d  "memgraph"\n)\nm
-00001e60: 656d 6772 6170 6820 3d20 6d65 6d67 7261  emgraph = memgra
-00001e70: 7068 5f69 6e73 7461 6e63 652e 7374 6172  ph_instance.star
-00001e80: 745f 616e 645f 636f 6e6e 6563 7428 7265  t_and_connect(re
-00001e90: 7374 6172 743d 4661 6c73 6529 5c6e 5c6e  start=False)\n\n
-00001ea0: 6d65 6d67 7261 7068 2e65 7865 6375 7465  memgraph.execute
-00001eb0: 5f61 6e64 5f66 6574 6368 2822 5245 5455  _and_fetch("RETU
-00001ec0: 524e 205c 274d 656d 6772 6170 6820 6973  RN \'Memgraph is
-00001ed0: 2072 756e 6e69 6e67 5c27 2041 5320 7265   running\' AS re
-00001ee0: 7375 6c74 2229 295b 305d 5b22 7265 7375  sult"))[0]["resu
-00001ef0: 6c74 225d 5c6e 6060 605c 6e3c 2f64 6574  lt"]\n```\n</det
-00001f00: 6169 6c73 3e5c 6e5c 6e3c 6465 7461 696c  ails>\n\n<detail
-00001f10: 733e 5c6e 3c73 756d 6d61 7279 3ef0 9f94  s>\n<summary>...
-00001f20: ab20 4d61 6e61 6765 2064 6174 6162 6173  . Manage databas
-00001f30: 6520 7472 6967 6765 7273 3c2f 7375 6d6d  e triggers</summ
-00001f40: 6172 793e 5c6e 3c62 723e 5c6e 5c6e 4265  ary>\n<br>\n\nBe
-00001f50: 6361 7573 6520 4d65 6d67 7261 7068 2073  cause Memgraph s
-00001f60: 7570 706f 7274 7320 6461 7461 6261 7365  upports database
-00001f70: 2074 7269 6767 6572 7320 6f6e 2060 4352   triggers on `CR
-00001f80: 4541 5445 602c 2060 5550 4441 5445 6020  EATE`, `UPDATE` 
-00001f90: 616e 6420 6044 454c 4554 4560 206f 7065  and `DELETE` ope
-00001fa0: 7261 7469 6f6e 732c 2047 514c 416c 6368  rations, GQLAlch
-00001fb0: 656d 7920 616c 736f 2069 6d70 6c65 6d65  emy also impleme
-00001fc0: 6e74 7320 6120 7369 6d70 6c65 2069 6e74  nts a simple int
-00001fd0: 6572 6661 6365 2066 6f72 206d 6169 6e74  erface for maint
-00001fe0: 6169 6e69 6e67 2074 6865 7365 2074 7269  aining these tri
-00001ff0: 6767 6572 732e 5c6e 5c6e 6060 6070 7974  ggers.\n\n```pyt
-00002000: 686f 6e5c 6e66 726f 6d20 6771 6c61 6c63  hon\nfrom gqlalc
-00002010: 6865 6d79 2069 6d70 6f72 7420 4d65 6d67  hemy import Memg
-00002020: 7261 7068 2c20 4d65 6d67 7261 7068 5472  raph, MemgraphTr
-00002030: 6967 6765 725c 6e66 726f 6d20 6771 6c61  igger\nfrom gqla
-00002040: 6c63 6865 6d79 2e6d 6f64 656c 7320 696d  lchemy.models im
-00002050: 706f 7274 2028 5c6e 2020 2020 5472 6967  port (\n    Trig
-00002060: 6765 7245 7665 6e74 5479 7065 2c5c 6e20  gerEventType,\n 
-00002070: 2020 2054 7269 6767 6572 4576 656e 744f     TriggerEventO
-00002080: 626a 6563 742c 5c6e 2020 2020 5472 6967  bject,\n    Trig
-00002090: 6765 7245 7865 6375 7469 6f6e 5068 6173  gerExecutionPhas
-000020a0: 652c 5c6e 295c 6e5c 6e64 6220 3d20 4d65  e,\n)\n\ndb = Me
-000020b0: 6d67 7261 7068 2829 5c6e 5c6e 7472 6967  mgraph()\n\ntrig
-000020c0: 6765 7220 3d20 4d65 6d67 7261 7068 5472  ger = MemgraphTr
-000020d0: 6967 6765 7228 5c6e 2020 2020 6e61 6d65  igger(\n    name
-000020e0: 3d22 7261 7469 6e67 735f 7472 6967 6765  ="ratings_trigge
-000020f0: 7222 2c5c 6e20 2020 2065 7665 6e74 5f74  r",\n    event_t
-00002100: 7970 653d 5472 6967 6765 7245 7665 6e74  ype=TriggerEvent
-00002110: 5479 7065 2e43 5245 4154 452c 5c6e 2020  Type.CREATE,\n  
-00002120: 2020 6576 656e 745f 6f62 6a65 6374 3d54    event_object=T
-00002130: 7269 6767 6572 4576 656e 744f 626a 6563  riggerEventObjec
-00002140: 742e 4e4f 4445 2c5c 6e20 2020 2065 7865  t.NODE,\n    exe
-00002150: 6375 7469 6f6e 5f70 6861 7365 3d54 7269  cution_phase=Tri
-00002160: 6767 6572 4578 6563 7574 696f 6e50 6861  ggerExecutionPha
-00002170: 7365 2e41 4654 4552 2c5c 6e20 2020 2073  se.AFTER,\n    s
-00002180: 7461 7465 6d65 6e74 3d22 554e 5749 4e44  tatement="UNWIND
-00002190: 2063 7265 6174 6564 5665 7274 6963 6573   createdVertices
-000021a0: 2041 5320 6e6f 6465 2053 4554 206e 6f64   AS node SET nod
-000021b0: 652e 6372 6561 7465 645f 6174 203d 204c  e.created_at = L
-000021c0: 6f63 616c 4461 7465 5469 6d65 2829 222c  ocalDateTime()",
-000021d0: 5c6e 295c 6e5c 6e64 622e 6372 6561 7465  \n)\n\ndb.create
-000021e0: 5f74 7269 6767 6572 2874 7269 6767 6572  _trigger(trigger
-000021f0: 295c 6e74 7269 6767 6572 7320 3d20 6462  )\ntriggers = db
-00002200: 2e67 6574 5f74 7269 6767 6572 7328 295c  .get_triggers()\
-00002210: 6e70 7269 6e74 2874 7269 6767 6572 7329  nprint(triggers)
-00002220: 5c6e 6060 605c 6e3c 2f64 6574 6169 6c73  \n```\n</details
-00002230: 3e5c 6e5c 6e3c 6465 7461 696c 733e 5c6e  >\n\n<details>\n
-00002240: 3c73 756d 6d61 7279 3ef0 9f92 bd20 4f6e  <summary>.... On
-00002250: 2d64 6973 6b20 7374 6f72 6167 653c 2f73  -disk storage</s
-00002260: 756d 6d61 7279 3e5c 6e3c 6272 3e5c 6e5c  ummary>\n<br>\n\
-00002270: 6e53 696e 6365 204d 656d 6772 6170 6820  nSince Memgraph 
-00002280: 6973 2061 6e20 696e 2d6d 656d 6f72 7920  is an in-memory 
-00002290: 6772 6170 6820 6461 7461 6261 7365 2c20  graph database, 
-000022a0: 7468 6520 4751 4c41 6c63 6865 6d79 206c  the GQLAlchemy l
-000022b0: 6962 7261 7279 2070 726f 7669 6465 7320  ibrary provides 
-000022c0: 616e 206f 6e2d 6469 736b 2073 746f 7261  an on-disk stora
-000022d0: 6765 2073 6f6c 7574 696f 6e20 666f 7220  ge solution for 
-000022e0: 6c61 7267 6520 7072 6f70 6572 7469 6573  large properties
-000022f0: 206e 6f74 2075 7365 6420 696e 2067 7261   not used in gra
-00002300: 7068 2061 6c67 6f72 6974 686d 732e 2054  ph algorithms. T
-00002310: 6869 7320 6973 2075 7365 6675 6c20 7768  his is useful wh
-00002320: 656e 206e 6f64 6573 206f 7220 7265 6c61  en nodes or rela
-00002330: 7469 6f6e 7368 6970 7320 6861 7665 206d  tionships have m
-00002340: 6574 6164 6174 6120 7468 6174 2064 6f65  etadata that doe
-00002350: 736e e280 9974 206e 6565 6420 746f 2062  sn...t need to b
-00002360: 6520 7573 6564 2069 6e20 616e 7920 6f66  e used in any of
-00002370: 2074 6865 2067 7261 7068 2061 6c67 6f72   the graph algor
-00002380: 6974 686d 7320 7468 6174 206e 6565 6420  ithms that need 
-00002390: 746f 2062 6520 6361 7272 6965 6420 6f75  to be carried ou
-000023a0: 7420 696e 204d 656d 6772 6170 682c 2062  t in Memgraph, b
-000023b0: 7574 2063 616e 2062 6520 6665 7463 6865  ut can be fetche
-000023c0: 6420 6166 7465 722e 204c 6561 726e 2061  d after. Learn a
-000023d0: 6c6c 2061 626f 7574 2069 7420 696e 2074  ll about it in t
-000023e0: 6865 205b 6f6e 2d64 6973 6b20 7374 6f72  he [on-disk stor
-000023f0: 6167 6520 686f 772d 746f 2067 7569 6465  age how-to guide
-00002400: 5d28 6874 7470 733a 2f2f 6d65 6d67 7261  ](https://memgra
-00002410: 7068 2e63 6f6d 2f64 6f63 732f 6771 6c61  ph.com/docs/gqla
-00002420: 6c63 6865 6d79 2f68 6f77 2d74 6f2d 6775  lchemy/how-to-gu
-00002430: 6964 6573 2f6f 6e2d 6469 736b 2d73 746f  ides/on-disk-sto
-00002440: 7261 6765 292e 5c6e 3c2f 6465 7461 696c  rage).\n</detail
-00002450: 733e 5c6e 5c6e 3c62 723e 5c6e 5c6e 4966  s>\n\n<br>\n\nIf
-00002460: 2079 6f75 2077 616e 7420 746f 206c 6561   you want to lea
-00002470: 726e 206d 6f72 6520 6162 6f75 7420 4f47  rn more about OG
-00002480: 4d2c 2071 7565 7279 2062 7569 6c64 6572  M, query builder
-00002490: 2c20 6d61 6e61 6769 6e67 2073 7472 6561  , managing strea
-000024a0: 6d73 2c20 696d 706f 7274 696e 6720 6461  ms, importing da
-000024b0: 7461 2066 726f 6d20 6469 6666 6572 656e  ta from differen
-000024c0: 7420 736f 7572 6365 2c20 6d61 6e61 6769  t source, managi
-000024d0: 6e67 204d 656d 6772 6170 6820 696e 7374  ng Memgraph inst
-000024e0: 616e 6365 732c 206d 616e 6167 696e 6720  ances, managing 
-000024f0: 6461 7461 6261 7365 2074 7269 6767 6572  database trigger
-00002500: 7320 616e 6420 7573 696e 6720 6f6e 2d64  s and using on-d
-00002510: 6973 6b20 7374 6f72 6167 652c 2063 6865  isk storage, che
-00002520: 636b 206f 7574 2074 6865 2047 514c 416c  ck out the GQLAl
-00002530: 6368 656d 7920 5b68 6f77 2d74 6f20 6775  chemy [how-to gu
-00002540: 6964 6573 5d28 6874 7470 733a 2f2f 6d65  ides](https://me
-00002550: 6d67 7261 7068 2e63 6f6d 2f64 6f63 732f  mgraph.com/docs/
-00002560: 6771 6c61 6c63 6865 6d79 2f68 6f77 2d74  gqlalchemy/how-t
-00002570: 6f2d 6775 6964 6573 292e 5c6e 5c6e 2323  o-guides).\n\n##
-00002580: 2044 6576 656c 6f70 6d65 6e74 2028 686f   Development (ho
-00002590: 7720 746f 2062 7569 6c64 295c 6e60 6060  w to build)\n```
-000025a0: 5c6e 706f 6574 7279 2072 756e 2066 6c61  \npoetry run fla
-000025b0: 6b65 3820 2e5c 6e70 6f65 7472 7920 7275  ke8 .\npoetry ru
-000025c0: 6e20 626c 6163 6b20 2e5c 6e70 6f65 7472  n black .\npoetr
-000025d0: 7920 7275 6e20 7079 7465 7374 202e 202d  y run pytest . -
-000025e0: 6b20 226e 6f74 2073 6c6f 7722 5c6e 6060  k "not slow"\n``
-000025f0: 605c 6e5c 6e23 2320 446f 6375 6d65 6e74  `\n\n## Document
-00002600: 6174 696f 6e5c 6e5c 6e54 6865 2047 514c  ation\n\nThe GQL
-00002610: 416c 6368 656d 7920 646f 6375 6d65 6e74  Alchemy document
-00002620: 6174 696f 6e20 6973 2061 7661 696c 6162  ation is availab
-00002630: 6c65 206f 6e20 5b6d 656d 6772 6170 682e  le on [memgraph.
-00002640: 636f 6d2f 646f 6373 2f67 716c 616c 6368  com/docs/gqlalch
-00002650: 656d 795d 2868 7474 7073 3a2f 2f6d 656d  emy](https://mem
-00002660: 6772 6170 682e 636f 6d2f 646f 6373 2f67  graph.com/docs/g
-00002670: 716c 616c 6368 656d 792f 292e 5c6e 5c6e  qlalchemy/).\n\n
-00002680: 5468 6520 646f 6375 6d65 6e74 6174 696f  The documentatio
-00002690: 6e20 6361 6e20 6265 2067 656e 6572 6174  n can be generat
-000026a0: 6564 2062 7920 6578 6563 7574 696e 673a  ed by executing:
-000026b0: 5c6e 6060 605c 6e70 6970 3320 696e 7374  \n```\npip3 inst
-000026c0: 616c 6c20 7079 7468 6f6e 2d6d 6172 6b64  all python-markd
-000026d0: 6f77 6e5c 6e70 7974 686f 6e2d 6d61 726b  own\npython-mark
-000026e0: 646f 776e 5c6e 6060 605c 6e5c 6e23 2320  down\n```\n\n## 
-000026f0: 4c69 6365 6e73 655c 6e5c 6e43 6f70 7972  License\n\nCopyr
-00002700: 6967 6874 2028 6329 2032 3031 362d 3230  ight (c) 2016-20
-00002710: 3232 205b 4d65 6d67 7261 7068 204c 7464  22 [Memgraph Ltd
-00002720: 2e5d 2868 7474 7073 3a2f 2f6d 656d 6772  .](https://memgr
-00002730: 6170 682e 636f 6d29 5c6e 5c6e 4c69 6365  aph.com)\n\nLice
-00002740: 6e73 6564 2075 6e64 6572 2074 6865 2041  nsed under the A
-00002750: 7061 6368 6520 4c69 6365 6e73 652c 2056  pache License, V
-00002760: 6572 7369 6f6e 2032 2e30 2028 7468 6520  ersion 2.0 (the 
-00002770: 224c 6963 656e 7365 2229 3b20 796f 7520  "License"); you 
-00002780: 6d61 7920 6e6f 7420 7573 655c 6e74 6869  may not use\nthi
-00002790: 7320 6669 6c65 2065 7863 6570 7420 696e  s file except in
-000027a0: 2063 6f6d 706c 6961 6e63 6520 7769 7468   compliance with
-000027b0: 2074 6865 204c 6963 656e 7365 2e20 596f   the License. Yo
-000027c0: 7520 6d61 7920 6f62 7461 696e 2061 2063  u may obtain a c
-000027d0: 6f70 7920 6f66 2074 6865 5c6e 4c69 6365  opy of the\nLice
-000027e0: 6e73 6520 6174 5c6e 5c6e 2020 2020 2068  nse at\n\n     h
-000027f0: 7474 703a 2f2f 7777 772e 6170 6163 6865  ttp://www.apache
-00002800: 2e6f 7267 2f6c 6963 656e 7365 732f 4c49  .org/licenses/LI
-00002810: 4345 4e53 452d 322e 305c 6e5c 6e55 6e6c  CENSE-2.0\n\nUnl
-00002820: 6573 7320 7265 7175 6972 6564 2062 7920  ess required by 
-00002830: 6170 706c 6963 6162 6c65 206c 6177 206f  applicable law o
-00002840: 7220 6167 7265 6564 2074 6f20 696e 2077  r agreed to in w
-00002850: 7269 7469 6e67 2c20 736f 6674 7761 7265  riting, software
-00002860: 2064 6973 7472 6962 7574 6564 5c6e 756e   distributed\nun
-00002870: 6465 7220 7468 6520 4c69 6365 6e73 6520  der the License 
-00002880: 6973 2064 6973 7472 6962 7574 6564 206f  is distributed o
-00002890: 6e20 616e 2022 4153 2049 5322 2042 4153  n an "AS IS" BAS
-000028a0: 4953 2c20 5749 5448 4f55 5420 5741 5252  IS, WITHOUT WARR
-000028b0: 414e 5449 4553 204f 525c 6e43 4f4e 4449  ANTIES OR\nCONDI
-000028c0: 5449 4f4e 5320 4f46 2041 4e59 204b 494e  TIONS OF ANY KIN
-000028d0: 442c 2065 6974 6865 7220 6578 7072 6573  D, either expres
-000028e0: 7320 6f72 2069 6d70 6c69 6564 2e20 5365  s or implied. Se
-000028f0: 6520 7468 6520 4c69 6365 6e73 6520 666f  e the License fo
-00002900: 7220 7468 655c 6e73 7065 6369 6669 6320  r the\nspecific 
-00002910: 6c61 6e67 7561 6765 2067 6f76 6572 6e69  language governi
-00002920: 6e67 2070 6572 6d69 7373 696f 6e73 2061  ng permissions a
-00002930: 6e64 206c 696d 6974 6174 696f 6e73 2075  nd limitations u
-00002940: 6e64 6572 2074 6865 204c 6963 656e 7365  nder the License
-00002950: 2e5c 6e27 2c0a 2020 2020 2761 7574 686f  .\n',.    'autho
-00002960: 7227 3a20 2742 7275 6e6f 2053 6163 6172  r': 'Bruno Sacar
-00002970: 6963 272c 0a20 2020 2027 6175 7468 6f72  ic',.    'author
-00002980: 5f65 6d61 696c 273a 2027 6272 756e 6f2e  _email': 'bruno.
-00002990: 7361 6361 7269 6340 6d65 6d67 7261 7068  sacaric@memgraph
-000029a0: 2e63 6f6d 272c 0a20 2020 2027 6d61 696e  .com',.    'main
-000029b0: 7461 696e 6572 273a 2027 4e6f 6e65 272c  tainer': 'None',
-000029c0: 0a20 2020 2027 6d61 696e 7461 696e 6572  .    'maintainer
-000029d0: 5f65 6d61 696c 273a 2027 4e6f 6e65 272c  _email': 'None',
-000029e0: 0a20 2020 2027 7572 6c27 3a20 2768 7474  .    'url': 'htt
-000029f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00002a00: 6d65 6d67 7261 7068 2f67 716c 616c 6368  memgraph/gqlalch
-00002a10: 656d 7927 2c0a 2020 2020 2770 6163 6b61  emy',.    'packa
-00002a20: 6765 7327 3a20 7061 636b 6167 6573 2c0a  ges': packages,.
-00002a30: 2020 2020 2770 6163 6b61 6765 5f64 6174      'package_dat
-00002a40: 6127 3a20 7061 636b 6167 655f 6461 7461  a': package_data
-00002a50: 2c0a 2020 2020 2769 6e73 7461 6c6c 5f72  ,.    'install_r
-00002a60: 6571 7569 7265 7327 3a20 696e 7374 616c  equires': instal
-00002a70: 6c5f 7265 7175 6972 6573 2c0a 2020 2020  l_requires,.    
-00002a80: 2770 7974 686f 6e5f 7265 7175 6972 6573  'python_requires
-00002a90: 273a 2027 3e3d 332e 382c 3c34 2e30 272c  ': '>=3.8,<4.0',
-00002aa0: 0a7d 0a0a 0a73 6574 7570 282a 2a73 6574  .}...setup(**set
-00002ab0: 7570 5f6b 7761 7267 7329 0a              up_kwargs).
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6771 6c61  : 2.1.Name: gqla
+00000020: 6c63 6865 6d79 0a56 6572 7369 6f6e 3a20  lchemy.Version: 
+00000030: 312e 342e 310a 5375 6d6d 6172 793a 2047  1.4.1.Summary: G
+00000040: 514c 416c 6368 656d 7920 6973 2061 206c  QLAlchemy is a l
+00000050: 6962 7261 7279 2064 6576 656c 6f70 6564  ibrary developed
+00000060: 2074 6f20 6173 7369 7374 2077 6974 6820   to assist with 
+00000070: 7772 6974 696e 6720 616e 6420 7275 6e6e  writing and runn
+00000080: 696e 6720 7175 6572 6965 7320 696e 204d  ing queries in M
+00000090: 656d 6772 6170 682e 0a48 6f6d 652d 7061  emgraph..Home-pa
+000000a0: 6765 3a20 6874 7470 733a 2f2f 6769 7468  ge: https://gith
+000000b0: 7562 2e63 6f6d 2f6d 656d 6772 6170 682f  ub.com/memgraph/
+000000c0: 6771 6c61 6c63 6865 6d79 0a4c 6963 656e  gqlalchemy.Licen
+000000d0: 7365 3a20 4170 6163 6865 2d32 2e30 0a41  se: Apache-2.0.A
+000000e0: 7574 686f 723a 2042 7275 6e6f 2053 6163  uthor: Bruno Sac
+000000f0: 6172 6963 0a41 7574 686f 722d 656d 6169  aric.Author-emai
+00000100: 6c3a 2062 7275 6e6f 2e73 6163 6172 6963  l: bruno.sacaric
+00000110: 406d 656d 6772 6170 682e 636f 6d0a 5265  @memgraph.com.Re
+00000120: 7175 6972 6573 2d50 7974 686f 6e3a 203e  quires-Python: >
+00000130: 3d33 2e38 2c3c 342e 300a 436c 6173 7369  =3.8,<4.0.Classi
+00000140: 6669 6572 3a20 4c69 6365 6e73 6520 3a3a  fier: License ::
+00000150: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000160: 2041 7061 6368 6520 536f 6674 7761 7265   Apache Software
+00000170: 204c 6963 656e 7365 0a43 6c61 7373 6966   License.Classif
+00000180: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00000190: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001a0: 686f 6e20 3a3a 2033 0a43 6c61 7373 6966  hon :: 3.Classif
+000001b0: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+000001c0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+000001d0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+000001e0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+000001f0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000200: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+00000210: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
+00000220: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000230: 2050 7974 686f 6e20 3a3a 2033 2e31 300a   Python :: 3.10.
+00000240: 436c 6173 7369 6669 6572 3a20 5072 6f67  Classifier: Prog
+00000250: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+00000260: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000270: 3131 0a50 726f 7669 6465 732d 4578 7472  11.Provides-Extr
+00000280: 613a 2061 6c6c 0a50 726f 7669 6465 732d  a: all.Provides-
+00000290: 4578 7472 613a 2061 7272 6f77 0a50 726f  Extra: arrow.Pro
+000002a0: 7669 6465 732d 4578 7472 613a 2064 676c  vides-Extra: dgl
+000002b0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
+000002c0: 2074 6f72 6368 2d70 7967 0a52 6571 7569   torch-pyg.Requi
+000002d0: 7265 732d 4469 7374 3a20 6164 6c66 7320  res-Dist: adlfs 
+000002e0: 283e 3d32 3032 322e 322e 302c 3c32 3032  (>=2022.2.0,<202
+000002f0: 332e 302e 3029 0a52 6571 7569 7265 732d  3.0.0).Requires-
+00000300: 4469 7374 3a20 6461 6369 7465 2028 3e3d  Dist: dacite (>=
+00000310: 312e 362e 302c 3c32 2e30 2e30 290a 5265  1.6.0,<2.0.0).Re
+00000320: 7175 6972 6573 2d44 6973 743a 2064 676c  quires-Dist: dgl
+00000330: 2028 3e3d 302e 392e 312c 3c30 2e31 302e   (>=0.9.1,<0.10.
+00000340: 3029 203b 2065 7874 7261 203d 3d20 2264  0) ; extra == "d
+00000350: 676c 2220 6f72 2065 7874 7261 203d 3d20  gl" or extra == 
+00000360: 2261 6c6c 220a 5265 7175 6972 6573 2d44  "all".Requires-D
+00000370: 6973 743a 2064 6f63 6b65 7220 283e 3d35  ist: docker (>=5
+00000380: 2e30 2e33 2c3c 362e 302e 3029 0a52 6571  .0.3,<6.0.0).Req
+00000390: 7569 7265 732d 4469 7374 3a20 6e65 6f34  uires-Dist: neo4
+000003a0: 6a20 283e 3d34 2e34 2e33 2c3c 352e 302e  j (>=4.4.3,<5.0.
+000003b0: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+000003c0: 3a20 6e65 7477 6f72 6b78 2028 3e3d 322e  : networkx (>=2.
+000003d0: 352e 312c 3c33 2e30 2e30 290a 5265 7175  5.1,<3.0.0).Requ
+000003e0: 6972 6573 2d44 6973 743a 206e 756d 7079  ires-Dist: numpy
+000003f0: 2028 3e3d 312e 3234 2e31 2c3c 322e 302e   (>=1.24.1,<2.0.
+00000400: 3029 0a52 6571 7569 7265 732d 4469 7374  0).Requires-Dist
+00000410: 3a20 7073 7574 696c 2028 3e3d 352e 392e  : psutil (>=5.9.
+00000420: 302c 3c36 2e30 2e30 290a 5265 7175 6972  0,<6.0.0).Requir
+00000430: 6573 2d44 6973 743a 2070 7961 7272 6f77  es-Dist: pyarrow
+00000440: 2028 3e3d 392e 302e 302c 3c31 302e 302e   (>=9.0.0,<10.0.
+00000450: 3029 203b 2065 7874 7261 203d 3d20 2261  0) ; extra == "a
+00000460: 7272 6f77 2220 6f72 2065 7874 7261 203d  rrow" or extra =
+00000470: 3d20 2261 6c6c 220a 5265 7175 6972 6573  = "all".Requires
+00000480: 2d44 6973 743a 2070 7964 616e 7469 6320  -Dist: pydantic 
+00000490: 283e 3d31 2e38 2e32 2c3c 322e 302e 3029  (>=1.8.2,<2.0.0)
+000004a0: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+000004b0: 7079 6d67 636c 6965 6e74 2028 3d3d 312e  pymgclient (==1.
+000004c0: 332e 3129 0a52 6571 7569 7265 732d 4469  3.1).Requires-Di
+000004d0: 7374 3a20 746f 7263 6820 283e 3d31 2e31  st: torch (>=1.1
+000004e0: 332e 312c 3c32 2e30 2e30 2920 3b20 6578  3.1,<2.0.0) ; ex
+000004f0: 7472 6120 3d3d 2022 6467 6c22 206f 7220  tra == "dgl" or 
+00000500: 6578 7472 6120 3d3d 2022 616c 6c22 206f  extra == "all" o
+00000510: 7220 6578 7472 6120 3d3d 2022 746f 7263  r extra == "torc
+00000520: 682d 7079 6722 0a50 726f 6a65 6374 2d55  h-pyg".Project-U
+00000530: 524c 3a20 5265 706f 7369 746f 7279 2c20  RL: Repository, 
+00000540: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000550: 6f6d 2f6d 656d 6772 6170 682f 6771 6c61  om/memgraph/gqla
+00000560: 6c63 6865 6d79 0a44 6573 6372 6970 7469  lchemy.Descripti
+00000570: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00000580: 2074 6578 742f 6d61 726b 646f 776e 0a0a   text/markdown..
+00000590: 2320 4751 4c41 6c63 6865 6d79 0a0a 0a3c  # GQLAlchemy...<
+000005a0: 703e 0a20 2020 203c 6120 6872 6566 3d22  p>.    <a href="
+000005b0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000005c0: 6f6d 2f6d 656d 6772 6170 682f 6771 6c61  om/memgraph/gqla
+000005d0: 6c63 6865 6d79 2f61 6374 696f 6e73 223e  lchemy/actions">
+000005e0: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+000005f0: 2f2f 6769 7468 7562 2e63 6f6d 2f6d 656d  //github.com/mem
+00000600: 6772 6170 682f 6771 6c61 6c63 6865 6d79  graph/gqlalchemy
+00000610: 2f77 6f72 6b66 6c6f 7773 2f42 7569 6c64  /workflows/Build
+00000620: 2532 3061 6e64 2532 3054 6573 742f 6261  %20and%20Test/ba
+00000630: 6467 652e 7376 6722 202f 3e3c 2f61 3e0a  dge.svg" /></a>.
+00000640: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+00000650: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000660: 6d65 6d67 7261 7068 2f67 716c 616c 6368  memgraph/gqlalch
+00000670: 656d 792f 626c 6f62 2f6d 6169 6e2f 4c49  emy/blob/main/LI
+00000680: 4345 4e53 4522 3e3c 696d 6720 7372 633d  CENSE"><img src=
+00000690: 2268 7474 7073 3a2f 2f69 6d67 2e73 6869  "https://img.shi
+000006a0: 656c 6473 2e69 6f2f 6769 7468 7562 2f6c  elds.io/github/l
+000006b0: 6963 656e 7365 2f6d 656d 6772 6170 682f  icense/memgraph/
+000006c0: 6771 6c61 6c63 6865 6d79 2220 2f3e 3c2f  gqlalchemy" /></
+000006d0: 613e 0a20 2020 203c 6120 6872 6566 3d22  a>.    <a href="
+000006e0: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+000006f0: 2f70 726f 6a65 6374 2f67 716c 616c 6368  /project/gqlalch
+00000700: 656d 7922 3e3c 696d 6720 7372 633d 2268  emy"><img src="h
+00000710: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000720: 6473 2e69 6f2f 7079 7069 2f76 2f67 716c  ds.io/pypi/v/gql
+00000730: 616c 6368 656d 7922 202f 3e3c 2f61 3e0a  alchemy" /></a>.
+00000740: 2020 2020 3c61 2068 7265 663d 2268 7474      <a href="htt
+00000750: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000760: 7073 662f 626c 6163 6b22 3e3c 696d 6720  psf/black"><img 
+00000770: 616c 743d 2243 6f64 6520 7374 796c 653a  alt="Code style:
+00000780: 2062 6c61 636b 2220 7372 633d 2268 7474   black" src="htt
+00000790: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+000007a0: 2e69 6f2f 6261 6467 652f 636f 6465 2532  .io/badge/code%2
+000007b0: 3073 7479 6c65 2d62 6c61 636b 2d30 3030  0style-black-000
+000007c0: 3030 302e 7376 6722 3e3c 2f61 3e0a 2020  000.svg"></a>.  
+000007d0: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
+000007e0: 3a2f 2f6d 656d 6772 6170 682e 636f 6d2f  ://memgraph.com/
+000007f0: 646f 6373 2f67 716c 616c 6368 656d 7922  docs/gqlalchemy"
+00000800: 2061 6c74 3d22 446f 6375 6d65 6e74 6174   alt="Documentat
+00000810: 696f 6e22 3e3c 696d 6720 7372 633d 2268  ion"><img src="h
+00000820: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+00000830: 6473 2e69 6f2f 6261 6467 652f 646f 6375  ds.io/badge/docu
+00000840: 6d65 6e74 6174 696f 6e2d 4751 4c41 6c63  mentation-GQLAlc
+00000850: 6865 6d79 2d6f 7261 6e67 6522 202f 3e3c  hemy-orange" /><
+00000860: 2f61 3e0a 2020 2020 3c61 2068 7265 663d  /a>.    <a href=
+00000870: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+00000880: 636f 6d2f 6d65 6d67 7261 7068 2f67 716c  com/memgraph/gql
+00000890: 616c 6368 656d 792f 7374 6172 6761 7a65  alchemy/stargaze
+000008a0: 7273 2220 616c 743d 2253 7461 7267 617a  rs" alt="Stargaz
+000008b0: 6572 7322 3e3c 696d 6720 7372 633d 2268  ers"><img src="h
+000008c0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000008d0: 6473 2e69 6f2f 6769 7468 7562 2f73 7461  ds.io/github/sta
+000008e0: 7273 2f6d 656d 6772 6170 682f 6771 6c61  rs/memgraph/gqla
+000008f0: 6c63 6865 6d79 3f73 7479 6c65 3d73 6f63  lchemy?style=soc
+00000900: 6961 6c22 202f 3e3c 2f61 3e0a 3c2f 703e  ial" /></a>.</p>
+00000910: 0a0a 2a2a 4751 4c41 6c63 6865 6d79 2a2a  ..**GQLAlchemy**
+00000920: 2069 7320 6120 6675 6c6c 7920 6f70 656e   is a fully open
+00000930: 2d73 6f75 7263 6520 5079 7468 6f6e 206c  -source Python l
+00000940: 6962 7261 7279 2061 6e64 202a 2a4f 626a  ibrary and **Obj
+00000950: 6563 7420 4772 6170 6820 4d61 7070 6572  ect Graph Mapper
+00000960: 2a2a 2028 4f47 4d29 202d 2061 206c 696e  ** (OGM) - a lin
+00000970: 6b20 6265 7477 6565 6e20 6772 6170 6820  k between graph 
+00000980: 6461 7461 6261 7365 206f 626a 6563 7473  database objects
+00000990: 2061 6e64 2050 7974 686f 6e20 6f62 6a65   and Python obje
+000009a0: 6374 732e 0a0a 416e 204f 626a 6563 7420  cts...An Object 
+000009b0: 4772 6170 6820 4d61 7070 6572 206f 7220  Graph Mapper or 
+000009c0: 4f47 4d20 7072 6f76 6964 6573 2061 2064  OGM provides a d
+000009d0: 6576 656c 6f70 6572 2d66 7269 656e 646c  eveloper-friendl
+000009e0: 7920 776f 726b 666c 6f77 2074 6861 7420  y workflow that 
+000009f0: 616c 6c6f 7773 2066 6f72 2077 7269 7469  allows for writi
+00000a00: 6e67 206f 626a 6563 742d 6f72 6965 6e74  ng object-orient
+00000a10: 6564 206e 6f74 6174 696f 6e20 746f 2063  ed notation to c
+00000a20: 6f6d 6d75 6e69 6361 7465 2077 6974 6820  ommunicate with 
+00000a30: 6772 6170 6820 6461 7461 6261 7365 732e  graph databases.
+00000a40: 2049 6e73 7465 6164 206f 6620 7772 6974   Instead of writ
+00000a50: 696e 6720 4379 7068 6572 2071 7565 7269  ing Cypher queri
+00000a60: 6573 2c20 796f 7520 7769 6c6c 2062 6520  es, you will be 
+00000a70: 6162 6c65 2074 6f20 7772 6974 6520 6f62  able to write ob
+00000a80: 6a65 6374 2d6f 7269 656e 7465 6420 636f  ject-oriented co
+00000a90: 6465 2c20 7768 6963 6820 7468 6520 4f47  de, which the OG
+00000aa0: 4d20 7769 6c6c 2061 7574 6f6d 6174 6963  M will automatic
+00000ab0: 616c 6c79 2074 7261 6e73 6c61 7465 2069  ally translate i
+00000ac0: 6e74 6f20 4379 7068 6572 2071 7565 7269  nto Cypher queri
+00000ad0: 6573 2e0a 0a23 2320 496e 7374 616c 6c61  es...## Installa
+00000ae0: 7469 6f6e 0a0a 4751 4c41 6c63 6865 6d79  tion..GQLAlchemy
+00000af0: 2069 7320 6275 696c 7420 6f6e 2074 6f70   is built on top
+00000b00: 206f 6620 4d65 6d67 7261 7068 2773 206c   of Memgraph's l
+00000b10: 6f77 2d6c 6576 656c 2050 7974 686f 6e20  ow-level Python 
+00000b20: 636c 6965 6e74 2060 7079 6d67 636c 6965  client `pymgclie
+00000b30: 6e74 600a 285b 5079 5049 5d28 6874 7470  nt`.([PyPI](http
+00000b40: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00000b50: 6a65 6374 2f70 796d 6763 6c69 656e 742f  ject/pymgclient/
+00000b60: 2920 2f0a 5b44 6f63 756d 656e 7461 7469  ) /.[Documentati
+00000b70: 6f6e 5d28 6874 7470 733a 2f2f 6d65 6d67  on](https://memg
+00000b80: 7261 7068 2e67 6974 6875 622e 696f 2f70  raph.github.io/p
+00000b90: 796d 6763 6c69 656e 742f 2920 2f0a 5b47  ymgclient/) /.[G
+00000ba0: 6974 4875 625d 2868 7474 7073 3a2f 2f67  itHub](https://g
+00000bb0: 6974 6875 622e 636f 6d2f 6d65 6d67 7261  ithub.com/memgra
+00000bc0: 7068 2f70 796d 6763 6c69 656e 7429 292e  ph/pymgclient)).
+00000bd0: 200a 0a54 6f20 696e 7374 616c 6c20 4751   ..To install GQ
+00000be0: 4c41 6c63 6865 6d79 2c20 796f 7520 6669  LAlchemy, you fi
+00000bf0: 7273 7420 6e65 6564 2074 6f20 696e 7374  rst need to inst
+00000c00: 616c 6c20 6070 796d 6763 6c69 656e 7460  all `pymgclient`
+00000c10: 205b 6275 696c 6420 7072 6572 6571 7569   [build prerequi
+00000c20: 7369 7465 735d 2868 7474 7073 3a2f 2f6d  sites](https://m
+00000c30: 656d 6772 6170 682e 6769 7468 7562 2e69  emgraph.github.i
+00000c40: 6f2f 7079 6d67 636c 6965 6e74 2f69 6e74  o/pymgclient/int
+00000c50: 726f 6475 6374 696f 6e2e 6874 6d6c 2362  roduction.html#b
+00000c60: 7569 6c64 2d70 7265 7265 7175 6973 6974  uild-prerequisit
+00000c70: 6573 292e 0a0a 4166 7465 7220 796f 7520  es)...After you 
+00000c80: 6861 7665 2069 6e73 7461 6c6c 6564 2074  have installed t
+00000c90: 6865 2070 7265 7265 7175 6973 6974 6573  he prerequisites
+00000ca0: 2c20 7275 6e20 7468 6520 666f 6c6c 6f77  , run the follow
+00000cb0: 696e 6720 636f 6d6d 616e 643a 0a0a 6070  ing command:..`p
+00000cc0: 6970 2069 6e73 7461 6c6c 2067 716c 616c  ip install gqlal
+00000cd0: 6368 656d 7960 0a0a 5769 7468 2074 6865  chemy`..With the
+00000ce0: 2061 626f 7665 2063 6f6d 6d61 6e64 2c20   above command, 
+00000cf0: 796f 7520 6765 7420 7468 6520 6261 7369  you get the basi
+00000d00: 6320 4751 4c41 6c63 6865 6d79 2063 6170  c GQLAlchemy cap
+00000d10: 6162 696c 6974 6965 732e 2054 6f20 6164  abilities. To ad
+00000d20: 6420 6164 6469 7469 6f6e 616c 2069 6d70  d additional imp
+00000d30: 6f72 742f 6578 706f 7274 2063 6170 6162  ort/export capab
+00000d40: 696c 6974 6965 732c 2069 6e73 7461 6c6c  ilities, install
+00000d50: 2047 514c 416c 6368 656d 7920 7769 7468   GQLAlchemy with
+00000d60: 206f 6e65 206f 6620 7468 6520 666f 6c6c   one of the foll
+00000d70: 6f77 696e 6720 636f 6d6d 616e 6473 3a0a  owing commands:.
+00000d80: 0a2d 2060 7069 7020 696e 7374 616c 6c20  .- `pip install 
+00000d90: 6771 6c61 6c63 6865 6d79 5b61 7272 6f77  gqlalchemy[arrow
+00000da0: 5d60 2023 2053 7570 706f 7274 2066 6f72  ]` # Support for
+00000db0: 2074 6865 2043 5356 2c20 5061 7271 7565   the CSV, Parque
+00000dc0: 742c 204f 5243 2061 6e64 2049 5043 2f46  t, ORC and IPC/F
+00000dd0: 6561 7468 6572 2f41 7272 6f77 2066 6f72  eather/Arrow for
+00000de0: 6d61 7473 0a2d 2060 7069 7020 696e 7374  mats.- `pip inst
+00000df0: 616c 6c20 6771 6c61 6c63 6865 6d79 5b64  all gqlalchemy[d
+00000e00: 676c 5d60 2023 2044 474c 2073 7570 706f  gl]` # DGL suppo
+00000e10: 7274 2028 696e 636c 7564 6573 2050 7954  rt (includes PyT
+00000e20: 6f72 6368 290a 0a2d 2060 7069 7020 696e  orch)..- `pip in
+00000e30: 7374 616c 6c20 6771 6c61 6c63 6865 6d79  stall gqlalchemy
+00000e40: 5b61 6c6c 5d60 2023 2041 6c6c 206f 6620  [all]` # All of 
+00000e50: 7468 6520 6162 6f76 650a 0a49 6620 796f  the above..If yo
+00000e60: 7520 696e 7465 6e64 2074 6f20 7573 6520  u intend to use 
+00000e70: 4751 4c41 6c63 6865 6d79 2077 6974 6820  GQLAlchemy with 
+00000e80: 5079 546f 7263 6820 4765 6f6d 6574 7269  PyTorch Geometri
+00000e90: 6320 7375 7070 6f72 742c 2074 6861 7420  c support, that 
+00000ea0: 6c69 6272 6172 7920 6d75 7374 2062 6520  library must be 
+00000eb0: 696e 7374 616c 6c65 6420 6d61 6e75 616c  installed manual
+00000ec0: 6c79 3a0a 0a60 6060 6261 7368 0a70 6970  ly:..```bash.pip
+00000ed0: 2069 6e73 7461 6c6c 2067 716c 616c 6368   install gqlalch
+00000ee0: 656d 795b 746f 7263 685f 7079 675d 2023  emy[torch_pyg] #
+00000ef0: 2070 7265 7265 7175 6973 6974 650a 7069   prerequisite.pi
+00000f00: 7020 696e 7374 616c 6c20 746f 7263 682d  p install torch-
+00000f10: 7363 6174 7465 7220 746f 7263 682d 7370  scatter torch-sp
+00000f20: 6172 7365 2074 6f72 6368 2d63 6c75 7374  arse torch-clust
+00000f30: 6572 2074 6f72 6368 2d73 706c 696e 652d  er torch-spline-
+00000f40: 636f 6e76 2074 6f72 6368 2d67 656f 6d65  conv torch-geome
+00000f50: 7472 6963 202d 6620 6874 7470 733a 2f2f  tric -f https://
+00000f60: 6461 7461 2e70 7967 2e6f 7267 2f77 686c  data.pyg.org/whl
+00000f70: 2f74 6f72 6368 2d31 2e31 332e 302b 6370  /torch-1.13.0+cp
+00000f80: 752e 6874 6d6c 220a 6060 600a 0a49 6620  u.html".```..If 
+00000f90: 796f 7520 6172 6520 7573 696e 6720 5b43  you are using [C
+00000fa0: 6f6e 6461 5d28 6874 7470 733a 2f2f 646f  onda](https://do
+00000fb0: 6373 2e63 6f6e 6461 2e69 6f2f 656e 2f6c  cs.conda.io/en/l
+00000fc0: 6174 6573 742f 2920 666f 7220 5079 7468  atest/) for Pyth
+00000fd0: 6f6e 2065 6e76 6972 6f6e 6d65 6e74 206d  on environment m
+00000fe0: 616e 6167 656d 656e 742c 2079 6f75 2063  anagement, you c
+00000ff0: 616e 2069 6e73 7461 6c6c 2047 514c 416c  an install GQLAl
+00001000: 6368 656d 7920 7468 726f 7567 6820 7069  chemy through pi
+00001010: 702e 0a0a 2323 2042 7569 6c64 2026 2054  p...## Build & T
+00001020: 6573 740a 0a54 6865 2070 726f 6a65 6374  est..The project
+00001030: 2075 7365 7320 5b50 6f65 7472 795d 2868   uses [Poetry](h
+00001040: 7474 7073 3a2f 2f70 7974 686f 6e2d 706f  ttps://python-po
+00001050: 6574 7279 2e6f 7267 2f29 2074 6f20 6275  etry.org/) to bu
+00001060: 696c 6420 7468 6520 6c69 6272 6172 792e  ild the library.
+00001070: 2043 6c6f 6e65 206f 7220 646f 776e 6c6f   Clone or downlo
+00001080: 6164 2074 6865 205b 4751 4c41 6c63 6865  ad the [GQLAlche
+00001090: 6d79 2073 6f75 7263 6520 636f 6465 5d28  my source code](
+000010a0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000010b0: 6f6d 2f6d 656d 6772 6170 682f 6771 6c61  om/memgraph/gqla
+000010c0: 6c63 6865 6d79 2920 6c6f 6361 6c6c 7920  lchemy) locally 
+000010d0: 616e 6420 7275 6e20 7468 6520 666f 6c6c  and run the foll
+000010e0: 6f77 696e 6720 636f 6d6d 616e 6420 746f  owing command to
+000010f0: 2062 7569 6c64 2069 7420 6672 6f6d 2073   build it from s
+00001100: 6f75 7263 6520 7769 7468 2050 6f65 7472  ource with Poetr
+00001110: 793a 0a0a 6060 6062 6173 680a 706f 6574  y:..```bash.poet
+00001120: 7279 2069 6e73 7461 6c6c 202d 2d61 6c6c  ry install --all
+00001130: 2d65 7874 7261 730a 6060 600a 0a54 6865  -extras.```..The
+00001140: 2060 6070 6f65 7472 7920 696e 7374 616c   ``poetry instal
+00001150: 6c20 2d2d 616c 6c2d 6578 7472 6173 6060  l --all-extras``
+00001160: 2063 6f6d 6d61 6e64 2069 6e73 7461 6c6c   command install
+00001170: 7320 4751 4c41 6c63 6865 6d79 2077 6974  s GQLAlchemy wit
+00001180: 6820 616c 6c20 6578 7472 6173 0a28 6f70  h all extras.(op
+00001190: 7469 6f6e 616c 2064 6570 656e 6465 6e63  tional dependenc
+000011a0: 6965 7329 2e20 416c 7465 726e 6174 6976  ies). Alternativ
+000011b0: 656c 792c 2079 6f75 2063 616e 2075 7365  ely, you can use
+000011c0: 2074 6865 2060 602d 4560 6020 6f70 7469   the ``-E`` opti
+000011d0: 6f6e 2074 6f20 6465 6669 6e65 0a77 6861  on to define.wha
+000011e0: 7420 6578 7472 6173 2074 6f20 696e 7374  t extras to inst
+000011f0: 616c 6c3a 0a0a 6060 6062 6173 680a 706f  all:..```bash.po
+00001200: 6574 7279 2069 6e73 7461 6c6c 2023 204e  etry install # N
+00001210: 6f20 6578 7472 6173 0a0a 706f 6574 7279  o extras..poetry
+00001220: 2069 6e73 7461 6c6c 202d 4520 6172 726f   install -E arro
+00001230: 7720 2320 5375 7070 6f72 7420 666f 7220  w # Support for 
+00001240: 7468 6520 4353 562c 2050 6172 7175 6574  the CSV, Parquet
+00001250: 2c20 4f52 4320 616e 6420 4950 432f 4665  , ORC and IPC/Fe
+00001260: 6174 6865 722f 4172 726f 7720 666f 726d  ather/Arrow form
+00001270: 6174 730a 706f 6574 7279 2069 6e73 7461  ats.poetry insta
+00001280: 6c6c 202d 4520 6467 6c20 2320 4447 4c20  ll -E dgl # DGL 
+00001290: 7375 7070 6f72 7420 2861 6c73 6f20 696e  support (also in
+000012a0: 636c 7564 6573 2074 6f72 6368 290a 6060  cludes torch).``
+000012b0: 600a 0a54 6f20 7275 6e20 7468 6520 7465  `..To run the te
+000012c0: 7374 732c 206d 616b 6520 7375 7265 2079  sts, make sure y
+000012d0: 6f75 2068 6176 6520 616e 205b 6163 7469  ou have an [acti
+000012e0: 7665 204d 656d 6772 6170 6820 696e 7374  ve Memgraph inst
+000012f0: 616e 6365 5d28 2f6d 656d 6772 6170 6829  ance](/memgraph)
+00001300: 2c20 616e 6420 6578 6563 7574 6520 6f6e  , and execute on
+00001310: 6520 6f66 2074 6865 2066 6f6c 6c6f 7769  e of the followi
+00001320: 6e67 2063 6f6d 6d61 6e64 733a 0a0a 6060  ng commands:..``
+00001330: 6062 6173 680a 706f 6574 7279 2072 756e  `bash.poetry run
+00001340: 2070 7974 6573 7420 2e20 2d6b 2022 6e6f   pytest . -k "no
+00001350: 7420 736c 6f77 2220 2320 4966 2061 6c6c  t slow" # If all
+00001360: 2065 7874 7261 7320 696e 7374 616c 6c65   extras installe
+00001370: 640a 0a70 6f65 7472 7920 7275 6e20 7079  d..poetry run py
+00001380: 7465 7374 202e 202d 6b20 226e 6f74 2073  test . -k "not s
+00001390: 6c6f 7720 616e 6420 6e6f 7420 6578 7472  low and not extr
+000013a0: 6173 2220 2320 4f74 6865 7277 6973 650a  as" # Otherwise.
+000013b0: 6060 600a 0a49 6620 796f 75e2 8099 7665  ```..If you...ve
+000013c0: 2069 6e73 7461 6c6c 6564 206f 6e6c 7920   installed only 
+000013d0: 6365 7274 6169 6e20 6578 7472 6173 2c20  certain extras, 
+000013e0: 6974 e280 9973 2061 6c73 6f20 706f 7373  it...s also poss
+000013f0: 6962 6c65 2074 6f20 7275 6e20 7468 6569  ible to run thei
+00001400: 7220 6173 736f 6369 6174 6564 2074 6573  r associated tes
+00001410: 7473 3a0a 0a60 6060 6261 7368 0a70 6f65  ts:..```bash.poe
+00001420: 7472 7920 7275 6e20 7079 7465 7374 202e  try run pytest .
+00001430: 202d 6b20 2261 7272 6f77 220a 706f 6574   -k "arrow".poet
+00001440: 7279 2072 756e 2070 7974 6573 7420 2e20  ry run pytest . 
+00001450: 2d6b 2022 6467 6c22 0a60 6060 0a0a 2323  -k "dgl".```..##
+00001460: 2047 514c 416c 6368 656d 7920 6361 7061   GQLAlchemy capa
+00001470: 6269 6c69 7469 6573 0a0a 3c64 6574 6169  bilities..<detai
+00001480: 6c73 3e0a 3c73 756d 6d61 7279 3ef0 9f97  ls>.<summary>...
+00001490: baef b88f 204f 626a 6563 7420 6772 6170  .... Object grap
+000014a0: 6820 6d61 7070 6572 3c2f 7375 6d6d 6172  h mapper</summar
+000014b0: 793e 0a3c 6272 3e0a 0a42 656c 6f77 2079  y>.<br>..Below y
+000014c0: 6f75 2063 616e 2073 6565 2061 6e20 6578  ou can see an ex
+000014d0: 616d 706c 6520 6f66 2068 6f77 2074 6f20  ample of how to 
+000014e0: 6372 6561 7465 2060 5573 6572 6020 616e  create `User` an
+000014f0: 6420 604c 616e 6775 6167 6560 206e 6f64  d `Language` nod
+00001500: 6520 636c 6173 7365 732c 2061 6e64 2061  e classes, and a
+00001510: 2072 656c 6174 696f 6e73 6869 7020 636c   relationship cl
+00001520: 6173 7320 6f66 2074 7970 6520 6053 5045  ass of type `SPE
+00001530: 414b 5360 2e20 416c 6f6e 6720 7769 7468  AKS`. Along with
+00001540: 2074 6861 742c 2079 6f75 2063 616e 2073   that, you can s
+00001550: 6565 2068 6f77 2074 6f20 6372 6561 7465  ee how to create
+00001560: 2061 206e 6577 206e 6f64 6520 616e 6420   a new node and 
+00001570: 7265 6c61 7469 6f6e 7368 6970 2061 6e64  relationship and
+00001580: 2068 6f77 2074 6f20 7361 7665 2074 6865   how to save the
+00001590: 6d20 696e 2074 6865 2064 6174 6162 6173  m in the databas
+000015a0: 652e 2041 6674 6572 2074 6861 742c 2079  e. After that, y
+000015b0: 6f75 2063 616e 206c 6f61 6420 7468 6f73  ou can load thos
+000015c0: 6520 6e6f 6465 7320 616e 6420 7265 6c61  e nodes and rela
+000015d0: 7469 6f6e 7368 6970 2066 726f 6d20 7468  tionship from th
+000015e0: 6520 6461 7461 6261 7365 2e0a 3c62 723e  e database..<br>
+000015f0: 0a3c 6272 3e0a 0a60 6060 7079 7468 6f6e  .<br>..```python
+00001600: 0a66 726f 6d20 6771 6c61 6c63 6865 6d79  .from gqlalchemy
+00001610: 2069 6d70 6f72 7420 4d65 6d67 7261 7068   import Memgraph
+00001620: 2c20 4e6f 6465 2c20 5265 6c61 7469 6f6e  , Node, Relation
+00001630: 7368 6970 2c20 4669 656c 640a 6672 6f6d  ship, Field.from
+00001640: 2074 7970 696e 6720 696d 706f 7274 204f   typing import O
+00001650: 7074 696f 6e61 6c0a 0a64 6220 3d20 4d65  ptional..db = Me
+00001660: 6d67 7261 7068 2829 0a0a 636c 6173 7320  mgraph()..class 
+00001670: 5573 6572 284e 6f64 652c 2069 6e64 6578  User(Node, index
+00001680: 3d54 7275 652c 2064 623d 6462 293a 0a20  =True, db=db):. 
+00001690: 2020 2069 643a 2073 7472 203d 2046 6965     id: str = Fie
+000016a0: 6c64 2869 6e64 6578 3d54 7275 652c 2065  ld(index=True, e
+000016b0: 7869 7374 3d54 7275 652c 2075 6e69 7175  xist=True, uniqu
+000016c0: 653d 5472 7565 2c20 6462 3d64 6229 0a0a  e=True, db=db)..
+000016d0: 636c 6173 7320 4c61 6e67 7561 6765 284e  class Language(N
+000016e0: 6f64 6529 3a0a 2020 2020 6e61 6d65 3a20  ode):.    name: 
+000016f0: 7374 7220 3d20 4669 656c 6428 756e 6971  str = Field(uniq
+00001700: 7565 3d54 7275 652c 2064 623d 6462 290a  ue=True, db=db).
+00001710: 0a63 6c61 7373 2053 7065 616b 7328 5265  .class Speaks(Re
+00001720: 6c61 7469 6f6e 7368 6970 2c20 7479 7065  lationship, type
+00001730: 3d22 5350 4541 4b53 2229 3a0a 2020 2020  ="SPEAKS"):.    
+00001740: 7061 7373 0a0a 7573 6572 203d 2055 7365  pass..user = Use
+00001750: 7228 6964 3d22 3322 2c20 7573 6572 6e61  r(id="3", userna
+00001760: 6d65 3d22 4a6f 686e 2229 2e73 6176 6528  me="John").save(
+00001770: 6462 290a 6c61 6e67 7561 6765 203d 204c  db).language = L
+00001780: 616e 6775 6167 6528 6e61 6d65 3d22 656e  anguage(name="en
+00001790: 2229 2e73 6176 6528 6462 290a 7370 6561  ").save(db).spea
+000017a0: 6b73 5f72 656c 203d 2053 7065 616b 7328  ks_rel = Speaks(
+000017b0: 0a20 2020 205f 7374 6172 745f 6e6f 6465  .    _start_node
+000017c0: 5f69 6420 3d20 7573 6572 2e5f 6964 2c0a  _id = user._id,.
+000017d0: 2020 2020 5f65 6e64 5f6e 6f64 655f 6964      _end_node_id
+000017e0: 203d 206c 616e 6775 6167 652e 5f69 640a   = language._id.
+000017f0: 292e 7361 7665 2864 6229 0a0a 6c6f 6164  ).save(db)..load
+00001800: 6564 5f75 7365 7220 3d20 5573 6572 2869  ed_user = User(i
+00001810: 643d 2233 2229 2e6c 6f61 6428 6462 3d64  d="3").load(db=d
+00001820: 6229 0a70 7269 6e74 286c 6f61 6465 645f  b).print(loaded_
+00001830: 7573 6572 290a 6c6f 6164 6564 5f73 7065  user).loaded_spe
+00001840: 616b 7320 3d20 5370 6561 6b73 280a 2020  aks = Speaks(.  
+00001850: 2020 2020 2020 5f73 7461 7274 5f6e 6f64        _start_nod
+00001860: 655f 6964 3d75 7365 722e 5f69 642c 0a20  e_id=user._id,. 
+00001870: 2020 2020 2020 205f 656e 645f 6e6f 6465         _end_node
+00001880: 5f69 643d 6c61 6e67 7561 6765 2e5f 6964  _id=language._id
+00001890: 0a20 2020 2029 2e6c 6f61 6428 6462 290a  .    ).load(db).
+000018a0: 7072 696e 7428 6c6f 6164 6564 5f73 7065  print(loaded_spe
+000018b0: 616b 7329 0a60 6060 0a3c 2f64 6574 6169  aks).```.</detai
+000018c0: 6c73 3e0a 0a3c 6465 7461 696c 733e 0a3c  ls>..<details>.<
+000018d0: 7375 6d6d 6172 793e f09f 94a8 2051 7565  summary>.... Que
+000018e0: 7279 2062 7569 6c64 6572 3c2f 7375 6d6d  ry builder</summ
+000018f0: 6172 793e 0a3c 6272 3e0a 5768 656e 2062  ary>.<br>.When b
+00001900: 7569 6c64 696e 6720 6120 4379 7068 6572  uilding a Cypher
+00001910: 2071 7565 7279 2c20 796f 7520 6361 6e20   query, you can 
+00001920: 7573 6520 6120 7365 7420 6f66 206d 6574  use a set of met
+00001930: 686f 6473 2074 6861 7420 6172 6520 7772  hods that are wr
+00001940: 6170 7065 7273 2061 726f 756e 6420 4379  appers around Cy
+00001950: 7068 6572 2063 6c61 7573 6573 2e20 0a3c  pher clauses. .<
+00001960: 6272 3e0a 3c62 723e 0a0a 6060 6070 7974  br>.<br>..```pyt
+00001970: 686f 6e0a 6672 6f6d 2067 716c 616c 6368  hon.from gqlalch
+00001980: 656d 7920 696d 706f 7274 2063 7265 6174  emy import creat
+00001990: 652c 206d 6174 6368 0a66 726f 6d20 6771  e, match.from gq
+000019a0: 6c61 6c63 6865 6d79 2e71 7565 7279 5f62  lalchemy.query_b
+000019b0: 7569 6c64 6572 2069 6d70 6f72 7420 4f70  uilder import Op
+000019c0: 6572 6174 6f72 0a0a 7175 6572 795f 6372  erator..query_cr
+000019d0: 6561 7465 203d 2063 7265 6174 6528 290a  eate = create().
+000019e0: 2020 2020 2020 2020 2e6e 6f64 6528 6c61          .node(la
+000019f0: 6265 6c73 3d22 5065 7273 6f6e 222c 206e  bels="Person", n
+00001a00: 616d 653d 224c 6573 6c69 6522 290a 2020  ame="Leslie").  
+00001a10: 2020 2020 2020 2e74 6f28 7265 6c61 7469        .to(relati
+00001a20: 6f6e 7368 6970 5f74 7970 653d 2246 5249  onship_type="FRI
+00001a30: 454e 4453 5f57 4954 4822 290a 2020 2020  ENDS_WITH").    
+00001a40: 2020 2020 2e6e 6f64 6528 6c61 6265 6c73      .node(labels
+00001a50: 3d22 5065 7273 6f6e 222c 206e 616d 653d  ="Person", name=
+00001a60: 2252 6f6e 2229 0a20 2020 2020 2020 202e  "Ron").        .
+00001a70: 6578 6563 7574 6528 290a 0a71 7565 7279  execute()..query
+00001a80: 5f6d 6174 6368 203d 206d 6174 6368 2829  _match = match()
+00001a90: 0a20 2020 2020 2020 202e 6e6f 6465 286c  .        .node(l
+00001aa0: 6162 656c 733d 2250 6572 736f 6e22 2c20  abels="Person", 
+00001ab0: 7661 7269 6162 6c65 3d22 7031 2229 0a20  variable="p1"). 
+00001ac0: 2020 2020 2020 202e 746f 2829 0a20 2020         .to().   
+00001ad0: 2020 2020 202e 6e6f 6465 286c 6162 656c       .node(label
+00001ae0: 733d 2250 6572 736f 6e22 2c20 7661 7269  s="Person", vari
+00001af0: 6162 6c65 3d22 7032 2229 0a20 2020 2020  able="p2").     
+00001b00: 2020 202e 7768 6572 6528 6974 656d 3d22     .where(item="
+00001b10: 7031 2e6e 616d 6522 2c20 6f70 6572 6174  p1.name", operat
+00001b20: 6f72 3d4f 7065 7261 746f 722e 4551 5541  or=Operator.EQUA
+00001b30: 4c2c 206c 6974 6572 616c 3d22 4c65 736c  L, literal="Lesl
+00001b40: 6965 2229 0a20 2020 2020 2020 202e 7265  ie").        .re
+00001b50: 7475 726e 5f28 7265 7375 6c74 733d 5b22  turn_(results=["
+00001b60: 7031 222c 2028 2270 3222 2c20 2273 6563  p1", ("p2", "sec
+00001b70: 6f6e 6422 295d 290a 2020 2020 2020 2020  ond")]).        
+00001b80: 2e65 7865 6375 7465 2829 0a60 6060 0a3c  .execute().```.<
+00001b90: 2f64 6574 6169 6c73 3e0a 0a3c 6465 7461  /details>..<deta
+00001ba0: 696c 733e 0a3c 7375 6d6d 6172 793e f09f  ils>.<summary>..
+00001bb0: 9ab0 204d 616e 6167 6520 7374 7265 616d  .. Manage stream
+00001bc0: 733c 2f73 756d 6d61 7279 3e0a 3c62 723e  s</summary>.<br>
+00001bd0: 0a0a 596f 7520 6361 6e20 6372 6561 7465  ..You can create
+00001be0: 2061 6e64 2073 7461 7274 204b 6166 6b61   and start Kafka
+00001bf0: 206f 7220 5075 6c73 6172 2073 7472 6561   or Pulsar strea
+00001c00: 6d20 7573 696e 6720 4751 4c41 6c63 6865  m using GQLAlche
+00001c10: 6d79 2e20 0a3c 6272 3e0a 0a2a 2a4b 6166  my. .<br>..**Kaf
+00001c20: 6b61 2073 7472 6561 6d2a 2a20 0a60 6060  ka stream** .```
+00001c30: 7079 7468 6f6e 0a66 726f 6d20 6771 6c61  python.from gqla
+00001c40: 6c63 6865 6d79 2069 6d70 6f72 7420 4d65  lchemy import Me
+00001c50: 6d67 7261 7068 4b61 666b 6153 7472 6561  mgraphKafkaStrea
+00001c60: 6d0a 0a73 7472 6561 6d20 3d20 4d65 6d67  m..stream = Memg
+00001c70: 7261 7068 4b61 666b 6153 7472 6561 6d28  raphKafkaStream(
+00001c80: 6e61 6d65 3d22 7261 7469 6e67 735f 7374  name="ratings_st
+00001c90: 7265 616d 222c 2074 6f70 6963 733d 5b22  ream", topics=["
+00001ca0: 7261 7469 6e67 7322 5d2c 2074 7261 6e73  ratings"], trans
+00001cb0: 666f 726d 3d22 6d6f 7669 656c 656e 732e  form="movielens.
+00001cc0: 7261 7469 6e67 222c 2062 6f6f 7473 7472  rating", bootstr
+00001cd0: 6170 5f73 6572 7665 7273 3d22 6c6f 6361  ap_servers="loca
+00001ce0: 6c68 6f73 743a 3930 3933 2229 0a64 622e  lhost:9093").db.
+00001cf0: 6372 6561 7465 5f73 7472 6561 6d28 7374  create_stream(st
+00001d00: 7265 616d 290a 6462 2e73 7461 7274 5f73  ream).db.start_s
+00001d10: 7472 6561 6d28 7374 7265 616d 290a 6060  tream(stream).``
+00001d20: 600a 0a0a 2a2a 5075 6c73 6172 2073 7472  `...**Pulsar str
+00001d30: 6561 6d2a 2a0a 6060 6070 7974 686f 6e0a  eam**.```python.
+00001d40: 6672 6f6d 2067 716c 616c 6368 656d 7920  from gqlalchemy 
+00001d50: 696d 706f 7274 204d 656d 6772 6170 6850  import MemgraphP
+00001d60: 756c 7361 7253 7472 6561 6d0a 0a73 7472  ulsarStream..str
+00001d70: 6561 6d20 3d20 4d65 6d67 7261 7068 5075  eam = MemgraphPu
+00001d80: 6c73 6172 5374 7265 616d 286e 616d 653d  lsarStream(name=
+00001d90: 2272 6174 696e 6773 5f73 7472 6561 6d22  "ratings_stream"
+00001da0: 2c20 746f 7069 6373 3d5b 2272 6174 696e  , topics=["ratin
+00001db0: 6773 225d 2c20 7472 616e 7366 6f72 6d3d  gs"], transform=
+00001dc0: 226d 6f76 6965 6c65 6e73 2e72 6174 696e  "movielens.ratin
+00001dd0: 6722 2c20 7365 7276 6963 655f 7572 6c3d  g", service_url=
+00001de0: 226c 6f63 616c 686f 7374 3a36 3635 3022  "localhost:6650"
+00001df0: 290a 6462 2e63 7265 6174 655f 7374 7265  ).db.create_stre
+00001e00: 616d 2873 7472 6561 6d29 0a64 622e 7374  am(stream).db.st
+00001e10: 6172 745f 7374 7265 616d 2873 7472 6561  art_stream(strea
+00001e20: 6d29 0a60 6060 0a0a 3c2f 6465 7461 696c  m).```..</detail
+00001e30: 733e 0a0a 3c64 6574 6169 6c73 3e0a 3c73  s>..<details>.<s
+00001e40: 756d 6d61 7279 3ef0 9f97 84ef b88f 2049  ummary>....... I
+00001e50: 6d70 6f72 7420 7461 626c 6520 6461 7461  mport table data
+00001e60: 2066 726f 6d20 6469 6666 6572 656e 7420   from different 
+00001e70: 736f 7572 6365 733c 2f73 756d 6d61 7279  sources</summary
+00001e80: 3e0a 3c62 723e 0a0a 2a2a 496d 706f 7274  >.<br>..**Import
+00001e90: 2074 6162 6c65 2064 6174 6120 746f 2061   table data to a
+00001ea0: 2067 7261 7068 2064 6174 6162 6173 652a   graph database*
+00001eb0: 2a0a 0a59 6f75 2063 616e 2074 7261 6e73  *..You can trans
+00001ec0: 6c61 7465 2074 6162 6c65 2064 6174 6120  late table data 
+00001ed0: 6672 6f6d 2061 2066 696c 6520 746f 2067  from a file to g
+00001ee0: 7261 7068 2064 6174 6120 616e 6420 696d  raph data and im
+00001ef0: 706f 7274 2069 7420 746f 204d 656d 6772  port it to Memgr
+00001f00: 6170 682e 2043 7572 7265 6e74 6c79 2c20  aph. Currently, 
+00001f10: 7765 2073 7570 706f 7274 2072 6561 6469  we support readi
+00001f20: 6e67 206f 6620 4353 562c 2050 6172 7175  ng of CSV, Parqu
+00001f30: 6574 2c20 4f52 4320 616e 6420 4950 432f  et, ORC and IPC/
+00001f40: 4665 6174 6865 722f 4172 726f 7720 6669  Feather/Arrow fi
+00001f50: 6c65 2066 6f72 6d61 7473 2076 6961 2074  le formats via t
+00001f60: 6865 2050 7941 7272 6f77 2070 6163 6b61  he PyArrow packa
+00001f70: 6765 2e0a 0a52 6561 6420 616c 6c20 6162  ge...Read all ab
+00001f80: 6f75 7420 6974 2069 6e20 5b74 6162 6c65  out it in [table
+00001f90: 2074 6f20 6772 6170 6820 696d 706f 7274   to graph import
+00001fa0: 6572 2068 6f77 2d74 6f20 6775 6964 655d  er how-to guide]
+00001fb0: 2868 7474 7073 3a2f 2f6d 656d 6772 6170  (https://memgrap
+00001fc0: 682e 636f 6d2f 646f 6373 2f67 716c 616c  h.com/docs/gqlal
+00001fd0: 6368 656d 792f 686f 772d 746f 2d67 7569  chemy/how-to-gui
+00001fe0: 6465 732f 7461 626c 652d 746f 2d67 7261  des/table-to-gra
+00001ff0: 7068 2d69 6d70 6f72 7465 7229 2e0a 0a2a  ph-importer)...*
+00002000: 2a4d 616b 6520 6120 6375 7374 6f6d 2066  *Make a custom f
+00002010: 696c 6520 7379 7374 656d 2069 6d70 6f72  ile system impor
+00002020: 7465 722a 2a0a 0a49 6620 796f 7520 7761  ter**..If you wa
+00002030: 6e74 2074 6f20 7265 6164 2066 726f 6d20  nt to read from 
+00002040: 6120 6669 6c65 2073 7973 7465 6d20 6e6f  a file system no
+00002050: 7420 6375 7272 656e 746c 7920 7375 7070  t currently supp
+00002060: 6f72 7465 6420 6279 2047 514c 416c 6368  orted by GQLAlch
+00002070: 656d 792c 206f 7220 7573 6520 6120 6669  emy, or use a fi
+00002080: 6c65 2074 7970 6520 6375 7272 656e 746c  le type currentl
+00002090: 7920 6e6f 7420 7265 6164 6162 6c65 2c20  y not readable, 
+000020a0: 796f 7520 6361 6e20 696d 706c 656d 656e  you can implemen
+000020b0: 7420 796f 7572 206f 776e 2062 7920 6578  t your own by ex
+000020c0: 7465 6e64 696e 6720 6162 7374 7261 6374  tending abstract
+000020d0: 2063 6c61 7373 6573 2060 4669 6c65 5379   classes `FileSy
+000020e0: 7374 656d 4861 6e64 6c65 7260 2061 6e64  stemHandler` and
+000020f0: 2060 4461 7461 4c6f 6164 6572 602c 2072   `DataLoader`, r
+00002100: 6573 7065 6374 6976 656c 792e 0a0a 5265  espectively...Re
+00002110: 6164 2061 6c6c 2061 626f 7574 2069 7420  ad all about it 
+00002120: 696e 205b 6375 7374 6f6d 2066 696c 6520  in [custom file 
+00002130: 7379 7374 656d 2069 6d70 6f72 7465 7220  system importer 
+00002140: 686f 772d 746f 2067 7569 6465 5d28 6874  how-to guide](ht
+00002150: 7470 733a 2f2f 6d65 6d67 7261 7068 2e63  tps://memgraph.c
+00002160: 6f6d 2f64 6f63 732f 6771 6c61 6c63 6865  om/docs/gqlalche
+00002170: 6d79 2f68 6f77 2d74 6f2d 6775 6964 6573  my/how-to-guides
+00002180: 2f63 7573 746f 6d2d 6669 6c65 2d73 7973  /custom-file-sys
+00002190: 7465 6d2d 696d 706f 7274 6572 292e 0a0a  tem-importer)...
+000021a0: 3c2f 6465 7461 696c 733e 0a0a 3c64 6574  </details>..<det
+000021b0: 6169 6c73 3e0a 3c73 756d 6d61 7279 3ee2  ails>.<summary>.
+000021c0: 9a99 efb8 8f20 4d61 6e61 6765 204d 656d  ..... Manage Mem
+000021d0: 6772 6170 6820 696e 7374 616e 6365 733c  graph instances<
+000021e0: 2f73 756d 6d61 7279 3e0a 3c62 723e 0a0a  /summary>.<br>..
+000021f0: 596f 7520 6361 6e20 7374 6172 742c 2073  You can start, s
+00002200: 746f 702c 2063 6f6e 6e65 6374 2074 6f20  top, connect to 
+00002210: 616e 6420 6d6f 6e69 746f 7220 4d65 6d67  and monitor Memg
+00002220: 7261 7068 2069 6e73 7461 6e63 6573 2077  raph instances w
+00002230: 6974 6820 4751 4c41 6c63 6865 6d79 2e0a  ith GQLAlchemy..
+00002240: 0a2a 2a4d 616e 6167 6520 4d65 6d67 7261  .**Manage Memgra
+00002250: 7068 2044 6f63 6b65 7220 696e 7374 616e  ph Docker instan
+00002260: 6365 2a2a 0a0a 6060 6070 7974 686f 6e0a  ce**..```python.
+00002270: 6672 6f6d 2067 716c 616c 6368 656d 792e  from gqlalchemy.
+00002280: 696e 7374 616e 6365 5f72 756e 6e65 7220  instance_runner 
+00002290: 696d 706f 7274 2028 0a20 2020 2044 6f63  import (.    Doc
+000022a0: 6b65 7249 6d61 6765 2c0a 2020 2020 4d65  kerImage,.    Me
+000022b0: 6d67 7261 7068 496e 7374 616e 6365 446f  mgraphInstanceDo
+000022c0: 636b 6572 0a29 0a0a 6d65 6d67 7261 7068  cker.)..memgraph
+000022d0: 5f69 6e73 7461 6e63 6520 3d20 4d65 6d67  _instance = Memg
+000022e0: 7261 7068 496e 7374 616e 6365 446f 636b  raphInstanceDock
+000022f0: 6572 280a 2020 2020 646f 636b 6572 5f69  er(.    docker_i
+00002300: 6d61 6765 3d44 6f63 6b65 7249 6d61 6765  mage=DockerImage
+00002310: 2e4d 454d 4752 4150 482c 2064 6f63 6b65  .MEMGRAPH, docke
+00002320: 725f 696d 6167 655f 7461 673d 226c 6174  r_image_tag="lat
+00002330: 6573 7422 2c20 686f 7374 3d22 302e 302e  est", host="0.0.
+00002340: 302e 3022 2c20 706f 7274 3d37 3638 370a  0.0", port=7687.
+00002350: 290a 6d65 6d67 7261 7068 203d 206d 656d  ).memgraph = mem
+00002360: 6772 6170 685f 696e 7374 616e 6365 2e73  graph_instance.s
+00002370: 7461 7274 5f61 6e64 5f63 6f6e 6e65 6374  tart_and_connect
+00002380: 2872 6573 7461 7274 3d46 616c 7365 290a  (restart=False).
+00002390: 0a6d 656d 6772 6170 682e 6578 6563 7574  .memgraph.execut
+000023a0: 655f 616e 645f 6665 7463 6828 2252 4554  e_and_fetch("RET
+000023b0: 5552 4e20 274d 656d 6772 6170 6820 6973  URN 'Memgraph is
+000023c0: 2072 756e 6e69 6e67 2720 4153 2072 6573   running' AS res
+000023d0: 756c 7422 2929 5b30 5d5b 2272 6573 756c  ult"))[0]["resul
+000023e0: 7422 5d0a 6060 600a 0a2a 2a4d 616e 6167  t"].```..**Manag
+000023f0: 6520 4d65 6d67 7261 7068 2062 696e 6172  e Memgraph binar
+00002400: 7920 696e 7374 616e 6365 2a2a 0a0a 6060  y instance**..``
+00002410: 6070 7974 686f 6e0a 6672 6f6d 2067 716c  `python.from gql
+00002420: 616c 6368 656d 792e 696e 7374 616e 6365  alchemy.instance
+00002430: 5f72 756e 6e65 7220 696d 706f 7274 204d  _runner import M
+00002440: 656d 6772 6170 6849 6e73 7461 6e63 6542  emgraphInstanceB
+00002450: 696e 6172 790a 0a6d 656d 6772 6170 685f  inary..memgraph_
+00002460: 696e 7374 616e 6365 203d 204d 656d 6772  instance = Memgr
+00002470: 6170 6849 6e73 7461 6e63 6542 696e 6172  aphInstanceBinar
+00002480: 7928 0a20 2020 2068 6f73 743d 2230 2e30  y(.    host="0.0
+00002490: 2e30 2e30 222c 2070 6f72 743d 3736 3938  .0.0", port=7698
+000024a0: 2c20 6269 6e61 7279 5f70 6174 683d 222f  , binary_path="/
+000024b0: 7573 722f 6c69 622f 6d65 6d67 7261 7068  usr/lib/memgraph
+000024c0: 2f6d 656d 6772 6170 6822 2c20 7573 6572  /memgraph", user
+000024d0: 3d22 6d65 6d67 7261 7068 220a 290a 6d65  ="memgraph".).me
+000024e0: 6d67 7261 7068 203d 206d 656d 6772 6170  mgraph = memgrap
+000024f0: 685f 696e 7374 616e 6365 2e73 7461 7274  h_instance.start
+00002500: 5f61 6e64 5f63 6f6e 6e65 6374 2872 6573  _and_connect(res
+00002510: 7461 7274 3d46 616c 7365 290a 0a6d 656d  tart=False)..mem
+00002520: 6772 6170 682e 6578 6563 7574 655f 616e  graph.execute_an
+00002530: 645f 6665 7463 6828 2252 4554 5552 4e20  d_fetch("RETURN 
+00002540: 274d 656d 6772 6170 6820 6973 2072 756e  'Memgraph is run
+00002550: 6e69 6e67 2720 4153 2072 6573 756c 7422  ning' AS result"
+00002560: 2929 5b30 5d5b 2272 6573 756c 7422 5d0a  ))[0]["result"].
+00002570: 6060 600a 3c2f 6465 7461 696c 733e 0a0a  ```.</details>..
+00002580: 3c64 6574 6169 6c73 3e0a 3c73 756d 6d61  <details>.<summa
+00002590: 7279 3ef0 9f94 ab20 4d61 6e61 6765 2064  ry>.... Manage d
+000025a0: 6174 6162 6173 6520 7472 6967 6765 7273  atabase triggers
+000025b0: 3c2f 7375 6d6d 6172 793e 0a3c 6272 3e0a  </summary>.<br>.
+000025c0: 0a42 6563 6175 7365 204d 656d 6772 6170  .Because Memgrap
+000025d0: 6820 7375 7070 6f72 7473 2064 6174 6162  h supports datab
+000025e0: 6173 6520 7472 6967 6765 7273 206f 6e20  ase triggers on 
+000025f0: 6043 5245 4154 4560 2c20 6055 5044 4154  `CREATE`, `UPDAT
+00002600: 4560 2061 6e64 2060 4445 4c45 5445 6020  E` and `DELETE` 
+00002610: 6f70 6572 6174 696f 6e73 2c20 4751 4c41  operations, GQLA
+00002620: 6c63 6865 6d79 2061 6c73 6f20 696d 706c  lchemy also impl
+00002630: 656d 656e 7473 2061 2073 696d 706c 6520  ements a simple 
+00002640: 696e 7465 7266 6163 6520 666f 7220 6d61  interface for ma
+00002650: 696e 7461 696e 696e 6720 7468 6573 6520  intaining these 
+00002660: 7472 6967 6765 7273 2e0a 0a60 6060 7079  triggers...```py
+00002670: 7468 6f6e 0a66 726f 6d20 6771 6c61 6c63  thon.from gqlalc
+00002680: 6865 6d79 2069 6d70 6f72 7420 4d65 6d67  hemy import Memg
+00002690: 7261 7068 2c20 4d65 6d67 7261 7068 5472  raph, MemgraphTr
+000026a0: 6967 6765 720a 6672 6f6d 2067 716c 616c  igger.from gqlal
+000026b0: 6368 656d 792e 6d6f 6465 6c73 2069 6d70  chemy.models imp
+000026c0: 6f72 7420 280a 2020 2020 5472 6967 6765  ort (.    Trigge
+000026d0: 7245 7665 6e74 5479 7065 2c0a 2020 2020  rEventType,.    
+000026e0: 5472 6967 6765 7245 7665 6e74 4f62 6a65  TriggerEventObje
+000026f0: 6374 2c0a 2020 2020 5472 6967 6765 7245  ct,.    TriggerE
+00002700: 7865 6375 7469 6f6e 5068 6173 652c 0a29  xecutionPhase,.)
+00002710: 0a0a 6462 203d 204d 656d 6772 6170 6828  ..db = Memgraph(
+00002720: 290a 0a74 7269 6767 6572 203d 204d 656d  )..trigger = Mem
+00002730: 6772 6170 6854 7269 6767 6572 280a 2020  graphTrigger(.  
+00002740: 2020 6e61 6d65 3d22 7261 7469 6e67 735f    name="ratings_
+00002750: 7472 6967 6765 7222 2c0a 2020 2020 6576  trigger",.    ev
+00002760: 656e 745f 7479 7065 3d54 7269 6767 6572  ent_type=Trigger
+00002770: 4576 656e 7454 7970 652e 4352 4541 5445  EventType.CREATE
+00002780: 2c0a 2020 2020 6576 656e 745f 6f62 6a65  ,.    event_obje
+00002790: 6374 3d54 7269 6767 6572 4576 656e 744f  ct=TriggerEventO
+000027a0: 626a 6563 742e 4e4f 4445 2c0a 2020 2020  bject.NODE,.    
+000027b0: 6578 6563 7574 696f 6e5f 7068 6173 653d  execution_phase=
+000027c0: 5472 6967 6765 7245 7865 6375 7469 6f6e  TriggerExecution
+000027d0: 5068 6173 652e 4146 5445 522c 0a20 2020  Phase.AFTER,.   
+000027e0: 2073 7461 7465 6d65 6e74 3d22 554e 5749   statement="UNWI
+000027f0: 4e44 2063 7265 6174 6564 5665 7274 6963  ND createdVertic
+00002800: 6573 2041 5320 6e6f 6465 2053 4554 206e  es AS node SET n
+00002810: 6f64 652e 6372 6561 7465 645f 6174 203d  ode.created_at =
+00002820: 204c 6f63 616c 4461 7465 5469 6d65 2829   LocalDateTime()
+00002830: 222c 0a29 0a0a 6462 2e63 7265 6174 655f  ",.)..db.create_
+00002840: 7472 6967 6765 7228 7472 6967 6765 7229  trigger(trigger)
+00002850: 0a74 7269 6767 6572 7320 3d20 6462 2e67  .triggers = db.g
+00002860: 6574 5f74 7269 6767 6572 7328 290a 7072  et_triggers().pr
+00002870: 696e 7428 7472 6967 6765 7273 290a 6060  int(triggers).``
+00002880: 600a 3c2f 6465 7461 696c 733e 0a0a 3c64  `.</details>..<d
+00002890: 6574 6169 6c73 3e0a 3c73 756d 6d61 7279  etails>.<summary
+000028a0: 3ef0 9f92 bd20 4f6e 2d64 6973 6b20 7374  >.... On-disk st
+000028b0: 6f72 6167 653c 2f73 756d 6d61 7279 3e0a  orage</summary>.
+000028c0: 3c62 723e 0a0a 5369 6e63 6520 4d65 6d67  <br>..Since Memg
+000028d0: 7261 7068 2069 7320 616e 2069 6e2d 6d65  raph is an in-me
+000028e0: 6d6f 7279 2067 7261 7068 2064 6174 6162  mory graph datab
+000028f0: 6173 652c 2074 6865 2047 514c 416c 6368  ase, the GQLAlch
+00002900: 656d 7920 6c69 6272 6172 7920 7072 6f76  emy library prov
+00002910: 6964 6573 2061 6e20 6f6e 2d64 6973 6b20  ides an on-disk 
+00002920: 7374 6f72 6167 6520 736f 6c75 7469 6f6e  storage solution
+00002930: 2066 6f72 206c 6172 6765 2070 726f 7065   for large prope
+00002940: 7274 6965 7320 6e6f 7420 7573 6564 2069  rties not used i
+00002950: 6e20 6772 6170 6820 616c 676f 7269 7468  n graph algorith
+00002960: 6d73 2e20 5468 6973 2069 7320 7573 6566  ms. This is usef
+00002970: 756c 2077 6865 6e20 6e6f 6465 7320 6f72  ul when nodes or
+00002980: 2072 656c 6174 696f 6e73 6869 7073 2068   relationships h
+00002990: 6176 6520 6d65 7461 6461 7461 2074 6861  ave metadata tha
+000029a0: 7420 646f 6573 6ee2 8099 7420 6e65 6564  t doesn...t need
+000029b0: 2074 6f20 6265 2075 7365 6420 696e 2061   to be used in a
+000029c0: 6e79 206f 6620 7468 6520 6772 6170 6820  ny of the graph 
+000029d0: 616c 676f 7269 7468 6d73 2074 6861 7420  algorithms that 
+000029e0: 6e65 6564 2074 6f20 6265 2063 6172 7269  need to be carri
+000029f0: 6564 206f 7574 2069 6e20 4d65 6d67 7261  ed out in Memgra
+00002a00: 7068 2c20 6275 7420 6361 6e20 6265 2066  ph, but can be f
+00002a10: 6574 6368 6564 2061 6674 6572 2e20 4c65  etched after. Le
+00002a20: 6172 6e20 616c 6c20 6162 6f75 7420 6974  arn all about it
+00002a30: 2069 6e20 7468 6520 5b6f 6e2d 6469 736b   in the [on-disk
+00002a40: 2073 746f 7261 6765 2068 6f77 2d74 6f20   storage how-to 
+00002a50: 6775 6964 655d 2868 7474 7073 3a2f 2f6d  guide](https://m
+00002a60: 656d 6772 6170 682e 636f 6d2f 646f 6373  emgraph.com/docs
+00002a70: 2f67 716c 616c 6368 656d 792f 686f 772d  /gqlalchemy/how-
+00002a80: 746f 2d67 7569 6465 732f 6f6e 2d64 6973  to-guides/on-dis
+00002a90: 6b2d 7374 6f72 6167 6529 2e0a 3c2f 6465  k-storage)..</de
+00002aa0: 7461 696c 733e 0a0a 3c62 723e 0a0a 4966  tails>..<br>..If
+00002ab0: 2079 6f75 2077 616e 7420 746f 206c 6561   you want to lea
+00002ac0: 726e 206d 6f72 6520 6162 6f75 7420 4f47  rn more about OG
+00002ad0: 4d2c 2071 7565 7279 2062 7569 6c64 6572  M, query builder
+00002ae0: 2c20 6d61 6e61 6769 6e67 2073 7472 6561  , managing strea
+00002af0: 6d73 2c20 696d 706f 7274 696e 6720 6461  ms, importing da
+00002b00: 7461 2066 726f 6d20 6469 6666 6572 656e  ta from differen
+00002b10: 7420 736f 7572 6365 2c20 6d61 6e61 6769  t source, managi
+00002b20: 6e67 204d 656d 6772 6170 6820 696e 7374  ng Memgraph inst
+00002b30: 616e 6365 732c 206d 616e 6167 696e 6720  ances, managing 
+00002b40: 6461 7461 6261 7365 2074 7269 6767 6572  database trigger
+00002b50: 7320 616e 6420 7573 696e 6720 6f6e 2d64  s and using on-d
+00002b60: 6973 6b20 7374 6f72 6167 652c 2063 6865  isk storage, che
+00002b70: 636b 206f 7574 2074 6865 2047 514c 416c  ck out the GQLAl
+00002b80: 6368 656d 7920 5b68 6f77 2d74 6f20 6775  chemy [how-to gu
+00002b90: 6964 6573 5d28 6874 7470 733a 2f2f 6d65  ides](https://me
+00002ba0: 6d67 7261 7068 2e63 6f6d 2f64 6f63 732f  mgraph.com/docs/
+00002bb0: 6771 6c61 6c63 6865 6d79 2f68 6f77 2d74  gqlalchemy/how-t
+00002bc0: 6f2d 6775 6964 6573 292e 0a0a 2323 2044  o-guides)...## D
+00002bd0: 6576 656c 6f70 6d65 6e74 2028 686f 7720  evelopment (how 
+00002be0: 746f 2062 7569 6c64 290a 0a60 6060 6261  to build)..```ba
+00002bf0: 7368 0a70 6f65 7472 7920 7275 6e20 666c  sh.poetry run fl
+00002c00: 616b 6538 202e 0a70 6f65 7472 7920 7275  ake8 ..poetry ru
+00002c10: 6e20 626c 6163 6b20 2e0a 706f 6574 7279  n black ..poetry
+00002c20: 2072 756e 2070 7974 6573 7420 2e20 2d6b   run pytest . -k
+00002c30: 2022 6e6f 7420 736c 6f77 2061 6e64 206e   "not slow and n
+00002c40: 6f74 2065 7874 7261 7322 0a60 6060 0a0a  ot extras".```..
+00002c50: 2323 2044 6f63 756d 656e 7461 7469 6f6e  ## Documentation
+00002c60: 0a0a 5468 6520 4751 4c41 6c63 6865 6d79  ..The GQLAlchemy
+00002c70: 2064 6f63 756d 656e 7461 7469 6f6e 2069   documentation i
+00002c80: 7320 6176 6169 6c61 626c 6520 6f6e 205b  s available on [
+00002c90: 6d65 6d67 7261 7068 2e63 6f6d 2f64 6f63  memgraph.com/doc
+00002ca0: 732f 6771 6c61 6c63 6865 6d79 5d28 6874  s/gqlalchemy](ht
+00002cb0: 7470 733a 2f2f 6d65 6d67 7261 7068 2e63  tps://memgraph.c
+00002cc0: 6f6d 2f64 6f63 732f 6771 6c61 6c63 6865  om/docs/gqlalche
+00002cd0: 6d79 2f29 2e0a 0a54 6865 2064 6f63 756d  my/)...The docum
+00002ce0: 656e 7461 7469 6f6e 2063 616e 2062 6520  entation can be 
+00002cf0: 6765 6e65 7261 7465 6420 6279 2065 7865  generated by exe
+00002d00: 6375 7469 6e67 3a0a 6060 600a 7069 7033  cuting:.```.pip3
+00002d10: 2069 6e73 7461 6c6c 2070 7964 6f63 2d6d   install pydoc-m
+00002d20: 6172 6b64 6f77 6e0a 7079 646f 632d 6d61  arkdown.pydoc-ma
+00002d30: 726b 646f 776e 0a60 6060 0a0a 2323 204c  rkdown.```..## L
+00002d40: 6963 656e 7365 0a0a 436f 7079 7269 6768  icense..Copyrigh
+00002d50: 7420 2863 2920 3230 3136 2d32 3032 3220  t (c) 2016-2022 
+00002d60: 5b4d 656d 6772 6170 6820 4c74 642e 5d28  [Memgraph Ltd.](
+00002d70: 6874 7470 733a 2f2f 6d65 6d67 7261 7068  https://memgraph
+00002d80: 2e63 6f6d 290a 0a4c 6963 656e 7365 6420  .com)..Licensed 
+00002d90: 756e 6465 7220 7468 6520 4170 6163 6865  under the Apache
+00002da0: 204c 6963 656e 7365 2c20 5665 7273 696f   License, Versio
+00002db0: 6e20 322e 3020 2874 6865 2022 4c69 6365  n 2.0 (the "Lice
+00002dc0: 6e73 6522 293b 2079 6f75 206d 6179 206e  nse"); you may n
+00002dd0: 6f74 2075 7365 0a74 6869 7320 6669 6c65  ot use.this file
+00002de0: 2065 7863 6570 7420 696e 2063 6f6d 706c   except in compl
+00002df0: 6961 6e63 6520 7769 7468 2074 6865 204c  iance with the L
+00002e00: 6963 656e 7365 2e20 596f 7520 6d61 7920  icense. You may 
+00002e10: 6f62 7461 696e 2061 2063 6f70 7920 6f66  obtain a copy of
+00002e20: 2074 6865 0a4c 6963 656e 7365 2061 740a   the.License at.
+00002e30: 0a20 2020 2020 6874 7470 3a2f 2f77 7777  .     http://www
+00002e40: 2e61 7061 6368 652e 6f72 672f 6c69 6365  .apache.org/lice
+00002e50: 6e73 6573 2f4c 4943 454e 5345 2d32 2e30  nses/LICENSE-2.0
+00002e60: 0a0a 556e 6c65 7373 2072 6571 7569 7265  ..Unless require
+00002e70: 6420 6279 2061 7070 6c69 6361 626c 6520  d by applicable 
+00002e80: 6c61 7720 6f72 2061 6772 6565 6420 746f  law or agreed to
+00002e90: 2069 6e20 7772 6974 696e 672c 2073 6f66   in writing, sof
+00002ea0: 7477 6172 6520 6469 7374 7269 6275 7465  tware distribute
+00002eb0: 640a 756e 6465 7220 7468 6520 4c69 6365  d.under the Lice
+00002ec0: 6e73 6520 6973 2064 6973 7472 6962 7574  nse is distribut
+00002ed0: 6564 206f 6e20 616e 2022 4153 2049 5322  ed on an "AS IS"
+00002ee0: 2042 4153 4953 2c20 5749 5448 4f55 5420   BASIS, WITHOUT 
+00002ef0: 5741 5252 414e 5449 4553 204f 520a 434f  WARRANTIES OR.CO
+00002f00: 4e44 4954 494f 4e53 204f 4620 414e 5920  NDITIONS OF ANY 
+00002f10: 4b49 4e44 2c20 6569 7468 6572 2065 7870  KIND, either exp
+00002f20: 7265 7373 206f 7220 696d 706c 6965 642e  ress or implied.
+00002f30: 2053 6565 2074 6865 204c 6963 656e 7365   See the License
+00002f40: 2066 6f72 2074 6865 0a73 7065 6369 6669   for the.specifi
+00002f50: 6320 6c61 6e67 7561 6765 2067 6f76 6572  c language gover
+00002f60: 6e69 6e67 2070 6572 6d69 7373 696f 6e73  ning permissions
+00002f70: 2061 6e64 206c 696d 6974 6174 696f 6e73   and limitations
+00002f80: 2075 6e64 6572 2074 6865 204c 6963 656e   under the Licen
+00002f90: 7365 2e0a 0a                             se...
```


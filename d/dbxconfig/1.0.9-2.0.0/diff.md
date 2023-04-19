# Comparing `tmp/dbxconfig-1.0.9.tar.gz` & `tmp/dbxconfig-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbxconfig-1.0.9.tar", last modified: Tue Apr 18 21:30:58 2023, max compression
+gzip compressed data, was "dbxconfig-2.0.0.tar", last modified: Wed Apr 19 11:38:07 2023, max compression
```

## Comparing `dbxconfig-1.0.9.tar` & `dbxconfig-2.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-18 21:30:58.691925 dbxconfig-1.0.9/
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-18 21:30:58.691925 dbxconfig-1.0.9/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     2936 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-18 21:30:58.691925 dbxconfig-1.0.9/dbxconfig/
--rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/dbxconfig/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1962 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/dbxconfig/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/dbxconfig/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      780 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/dbxconfig/_table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3479 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/dbxconfig/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/dbxconfig/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1836 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/dbxconfig/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-18 21:30:58.691925 dbxconfig-1.0.9/dbxconfig/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/dbxconfig/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      869 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/dbxconfig/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3088 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/dbxconfig/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2680 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/dbxconfig/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4910 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/dbxconfig/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/dbxconfig/dataset/_write.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-18 21:30:58.691925 dbxconfig-1.0.9/dbxconfig.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-18 21:30:58.000000 dbxconfig-1.0.9/dbxconfig.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      544 2023-04-18 21:30:58.000000 dbxconfig-1.0.9/dbxconfig.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-18 21:30:58.000000 dbxconfig-1.0.9/dbxconfig.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-18 21:30:58.000000 dbxconfig-1.0.9/dbxconfig.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-04-18 21:30:58.000000 dbxconfig-1.0.9/dbxconfig.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-18 21:30:58.000000 dbxconfig-1.0.9/dbxconfig.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-18 21:30:58.691925 dbxconfig-1.0.9/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1103 2023-04-18 21:30:06.000000 dbxconfig-1.0.9/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 11:38:07.439487 dbxconfig-2.0.0/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-19 11:38:07.439487 dbxconfig-2.0.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     2936 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 11:38:07.439487 dbxconfig-2.0.0/dbxconfig/
+-rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/dbxconfig/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2764 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/dbxconfig/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      166 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/dbxconfig/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      780 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/dbxconfig/_table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3513 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/dbxconfig/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/dbxconfig/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1979 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/dbxconfig/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 11:38:07.439487 dbxconfig-2.0.0/dbxconfig/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      200 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/dbxconfig/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      903 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/dbxconfig/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3088 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/dbxconfig/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2781 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/dbxconfig/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4982 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/dbxconfig/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/dbxconfig/dataset/_write.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-04-19 11:38:07.439487 dbxconfig-2.0.0/dbxconfig.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3488 2023-04-19 11:38:07.000000 dbxconfig-2.0.0/dbxconfig.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      544 2023-04-19 11:38:07.000000 dbxconfig-2.0.0/dbxconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-19 11:38:07.000000 dbxconfig-2.0.0/dbxconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-04-19 11:38:07.000000 dbxconfig-2.0.0/dbxconfig.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       31 2023-04-19 11:38:07.000000 dbxconfig-2.0.0/dbxconfig.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-04-19 11:38:07.000000 dbxconfig-2.0.0/dbxconfig.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-04-19 11:38:07.439487 dbxconfig-2.0.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1103 2023-04-19 11:37:15.000000 dbxconfig-2.0.0/setup.py
```

### Comparing `dbxconfig-1.0.9/PKG-INFO` & `dbxconfig-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 1.0.9
+Version: 2.0.0
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-1.0.9/README.md` & `dbxconfig-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.9/dbxconfig/_config.py` & `dbxconfig-2.0.0/dbxconfig/_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,59 @@
 import yaml
 import os
 from .dataset import DataSet
 from ._timeslice import Timeslice
 from ._tables import Tables, _INDEX_WILDCARD
 from ._stage_type import StageType
 from .dataset import dataset_factory
+from ._utils import abs_config_path
 
 
 class Config:
-    _CONFIG_PATH = "../Config/"
-    _CONFIG_FILE = "config.yaml"
+    _CONFIG_PATH = "./Config/"
     _ENCODING = "utf-8"
     _TABLES = "tables"
     _SOURCE_TABLE = "source_table"
 
-    def __init__(self, config_path: str = None):
-        self.config = {}
+    def __init__(self, pattern: str, config_path: str = None):
+        self.config = self._load_config(pattern, config_path)
+        self.tables = self._load_tables()
 
-        if not config_path:
-            config_path = os.path.join(self._CONFIG_PATH, self._CONFIG_FILE)
+    def _load_config(self, pattern: str, config_path: str):
+        config_path = self._get_config_path(config_path)
+        config_file = f"{pattern}.yaml"
+
+        config_file_path = os.path.join(config_path, config_file)
 
-        with open(config_path, "r", encoding=self._ENCODING) as f:
-            self.config = yaml.safe_load(f)
+        with open(config_file_path, "r", encoding=self._ENCODING) as f:
+            config = yaml.safe_load(f)
 
-        _tables_path = self.config["tables"]
+        # add the configuration path into the confif dictionart
+        # so that it gets passed to table config when created
+        config["config_path"] = config_path
+        return config
 
-        with open(_tables_path, "r", encoding=self._ENCODING) as f:
+    def _load_tables(self):
+        tables_path = self.config["tables"]
+        tables_path = abs_config_path(self.config["config_path"], self.config["tables"])
+
+        with open(tables_path, "r", encoding=self._ENCODING) as f:
             self.config["tables"] = yaml.safe_load(f)
 
-        self.tables = Tables(table_data=self.config["tables"])
+        tables = Tables(
+            table_data=self.config["tables"], config_path=self.config["config_path"]
+        )
+
+        return tables
+
+    def _get_config_path(self, config_path: str):
+        if not config_path:
+            config_path = self._CONFIG_PATH
+        config_path = os.path.abspath(config_path)
+        return config_path
 
     def get_table_mapping(
         self,
         timeslice: Timeslice,
         stage: StageType,
         table: str = _INDEX_WILDCARD,
         database: str = _INDEX_WILDCARD,
@@ -47,15 +68,15 @@
         )
         table_mapping.destination = dataset_factory.get_data_set(
             self.config, table_mapping.destination, timeslice
         )
 
         return table_mapping
 
-    def link_checkpoint(
+    def set_checkpoint(
         self,
         source: DataSet,
         destination: DataSet,
         checkpoint_name: str = None,
     ):
         if not checkpoint_name:
             checkpoint_name = f"{source.database}.{source.table}-{destination.database}.{destination.table}"
```

### Comparing `dbxconfig-1.0.9/dbxconfig/_table.py` & `dbxconfig-2.0.0/dbxconfig/_table.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.9/dbxconfig/_tables.py` & `dbxconfig-2.0.0/dbxconfig/_tables.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._load_index()
 
     table_data: dict = Field(...)
     tables_index: Dict[str, Table] = Field(default={})
     table_properties: Dict[str, str] = Field(default=None)
+    config_path: str = Field(...)
 
     @classmethod
     def get_index(
         cls,
         stage: Union[StageType, str] = _INDEX_WILDCARD,
         table=_INDEX_WILDCARD,
         database=_INDEX_WILDCARD,
```

### Comparing `dbxconfig-1.0.9/dbxconfig/_timeslice.py` & `dbxconfig-2.0.0/dbxconfig/_timeslice.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.9/dbxconfig/_utils.py` & `dbxconfig-2.0.0/dbxconfig/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import jinja2
 from enum import Enum
 import yaml
 from pyspark.sql.types import StructType
 from typing import Dict
+import os
 
 
 class JinjaVariables(Enum):
     DATABASE = "database"
     TABLE = "table"
     CHECKPOINT = "checkpoint"
     FILENAME_DATE_FORMAT = "filename_date_format"
@@ -26,14 +27,20 @@
         if not skip:
             template: jinja2.Template = jinja2.Template(data)
             data = template.render(replace)
 
     return data
 
 
+def abs_config_path(root: str, path: str):
+    if not os.path.isabs(path):
+        path = os.path.join(root, path)
+    return path
+
+
 def load_schema(path: str):
     with open(path, "r", encoding="utf-8") as f:
         schema = yaml.safe_load(f)
 
     schema = StructType.fromJson(schema)
 
     return schema
```

### Comparing `dbxconfig-1.0.9/dbxconfig/dataset/_dataset.py` & `dbxconfig-2.0.0/dbxconfig/dataset/_dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,10 +19,11 @@
     container: str = Field(...)
     root: str = Field(...)
     path: str = Field(default=None)
     options: dict = Field(...)
     timeslice: Timeslice = Field(...)
     checkpoint: str = Field(default=None)
     stage: StageType = Field(...)
+    config_path: str = Field(...)
 
     def _render(self):
         pass
```

### Comparing `dbxconfig-1.0.9/dbxconfig/dataset/_deltalake.py` & `dbxconfig-2.0.0/dbxconfig/dataset/_deltalake.py`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.9/dbxconfig/dataset/_factory.py` & `dbxconfig-2.0.0/dbxconfig/dataset/_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 class _DatasetFactory:
     _TIMESLICE = "timeslice"
     _TABLE = "destination_table"
     _TABLE_PROPERTIES = "table_properties"
     _STAGE = "stage"
     _DATABASE = "database"
+    _CONFIG_PATH = "config_path"
 
     def __init__(self) -> None:
         self._logger = logging.getLogger(self.__class__.__name__)
         self._dataset = {}
 
     def register_dataset_type(self, io_type: StageType, dataset_type: type):
         self._logger.debug(f"Register dataset type {dataset_type} as {type}")
@@ -70,14 +71,15 @@
     def _get_stage_table_config(self, config: dict, table: Table, timeslice: Timeslice):
         stage_config = config[table.stage.name]
         stage_config[self._TIMESLICE] = timeslice
         stage_config[self._TABLE] = table.name
         stage_config[self._TABLE_PROPERTIES] = table.table_properties
         stage_config[self._STAGE] = table.stage
         stage_config[self._DATABASE] = table.database
+        stage_config[self._CONFIG_PATH] = config[self._CONFIG_PATH]
 
         return stage_config
 
 
 factory = _DatasetFactory()
 factory.register_dataset_type(IOType.READ, Read)
 factory.register_dataset_type(IOType.DELTALAKE, DeltaLake)
```

### Comparing `dbxconfig-1.0.9/dbxconfig/dataset/_read.py` & `dbxconfig-2.0.0/dbxconfig/dataset/_read.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from pydantic import Field, PrivateAttr
-from .._utils import JinjaVariables, render_jinja, get_ddl, load_schema
+from .._utils import JinjaVariables, render_jinja, get_ddl, load_schema, abs_config_path
 from typing import Any, Dict, List, Union
 from .._timeslice import Timeslice
 from enum import Enum
 import os
 from pyspark.sql.types import StructType
 from pyspark.sql.streaming import StreamingQuery
 from pyspark.sql import DataFrame
@@ -93,14 +93,15 @@
                 self.options[self._OPTION_CF_SCHEMA_HINTS] = ", ".join(self.ddl)
             else:
                 self.options[self._OPTION_CF_SCHEMA_HINTS] = ", ".join(
                     self.headerless_ddl
                 )
 
     def _load_schema(self, path: str):
+        path = abs_config_path(self.config_path, path)
         if not self.spark_schema or isinstance(self.spark_schema, str):
             self.spark_schema = load_schema(path)
         if not self.ddl:
             self.ddl = get_ddl(self.spark_schema, header=True)
         if not self.headerless_ddl:
             self.headerless_ddl = get_ddl(self.spark_schema, header=False)
```

### Comparing `dbxconfig-1.0.9/dbxconfig.egg-info/PKG-INFO` & `dbxconfig-2.0.0/dbxconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbxconfig
-Version: 1.0.9
+Version: 2.0.0
 Summary: Databricks Configuration Framework
 Home-page: https://dbxconfig.readthedocs.io/en/latest/
 Author: Shaun Ryan
 Author-email: shaun_chiburi@hotmail.com
 License: MIT
 Project-URL: GitHub, https://github.com/semanticinsight/dbxconfig
 Project-URL: Documentation, https://dbxconfig.readthedocs.io/en/latest/
```

### Comparing `dbxconfig-1.0.9/dbxconfig.egg-info/SOURCES.txt` & `dbxconfig-2.0.0/dbxconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbxconfig-1.0.9/setup.py` & `dbxconfig-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="dbxconfig",
-    version="1.0.9",
+    version="2.0.0",
     description="Databricks Configuration Framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://dbxconfig.readthedocs.io/en/latest/",
     project_urls={
         'GitHub': 'https://github.com/semanticinsight/dbxconfig',
         'Documentation': 'https://dbxconfig.readthedocs.io/en/latest/'
```


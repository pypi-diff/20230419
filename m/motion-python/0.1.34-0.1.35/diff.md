# Comparing `tmp/motion_python-0.1.34.tar.gz` & `tmp/motion_python-0.1.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.34.tar", max compression
+gzip compressed data, was "motion_python-0.1.35.tar", max compression
```

## Comparing `motion_python-0.1.34.tar` & `motion_python-0.1.35.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3232 2023-04-14 05:05:49.085532 motion_python-0.1.34/README.md
--rw-r--r--   0        0        0      671 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/__init__.py
--rw-r--r--   0        0        0       80 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/api/__init__.py
--rw-r--r--   0        0        0     6684 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/api/api.py
--rw-r--r--   0        0        0      616 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/api/models.py
--rw-r--r--   0        0        0     3776 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/cli.py
--rw-r--r--   0        0        0    10092 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/client.py
--rw-r--r--   0        0        0    22271 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/cursor.py
--rw-r--r--   0        0        0    10037 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/entry.py
--rw-r--r--   0        0        0      214 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/basic/mconfig.py
--rw-r--r--   0        0        0        0 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/basic/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/basic/triggers/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/dashboard.py
--rw-r--r--   0        0        0      388 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/mconfig.py
--rw-r--r--   0        0        0       63 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/requirements.txt
--rw-r--r--   0        0        0       73 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/schemas/__init__.py
--rw-r--r--   0        0        0      398 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/schemas/all.py
--rw-r--r--   0        0        0     1377 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/test.py
--rw-r--r--   0        0        0      134 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/triggers/__init__.py
--rw-r--r--   0        0        0     4617 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/triggers/scrape.py
--rw-r--r--   0        0        0     5003 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/examples/cooking/triggers/search.py
--rw-r--r--   0        0        0     2975 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/routing.py
--rw-r--r--   0        0        0     3413 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/schema.py
--rw-r--r--   0        0        0    15114 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/store.py
--rw-r--r--   0        0        0     3746 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/task.py
--rw-r--r--   0        0        0     6058 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/trigger.py
--rw-r--r--   0        0        0     1892 2023-04-14 05:05:49.089532 motion_python-0.1.34/motion/utils.py
--rw-r--r--   0        0        0     1578 2023-04-14 05:06:10.133161 motion_python-0.1.34/pyproject.toml
--rw-r--r--   0        0        0     4405 1970-01-01 00:00:00.000000 motion_python-0.1.34/PKG-INFO
+-rw-r--r--   0        0        0     3232 2023-04-19 17:21:20.053974 motion_python-0.1.35/README.md
+-rw-r--r--   0        0        0      671 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/__init__.py
+-rw-r--r--   0        0        0       80 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/api/__init__.py
+-rw-r--r--   0        0        0     6684 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/api/api.py
+-rw-r--r--   0        0        0      616 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/api/models.py
+-rw-r--r--   0        0        0     3951 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/cli.py
+-rw-r--r--   0        0        0    10092 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/client.py
+-rw-r--r--   0        0        0    22261 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/cursor.py
+-rw-r--r--   0        0        0    10037 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/entry.py
+-rw-r--r--   0        0        0      214 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/basic/mconfig.py
+-rw-r--r--   0        0        0        0 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/basic/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/basic/triggers/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/dashboard.py
+-rw-r--r--   0        0        0      388 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/mconfig.py
+-rw-r--r--   0        0        0       63 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/requirements.txt
+-rw-r--r--   0        0        0       73 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/schemas/__init__.py
+-rw-r--r--   0        0        0      398 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/schemas/all.py
+-rw-r--r--   0        0        0     1377 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/test.py
+-rw-r--r--   0        0        0      134 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/triggers/__init__.py
+-rw-r--r--   0        0        0     4617 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/triggers/scrape.py
+-rw-r--r--   0        0        0     5003 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/examples/cooking/triggers/search.py
+-rw-r--r--   0        0        0     2975 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/routing.py
+-rw-r--r--   0        0        0     3413 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/schema.py
+-rw-r--r--   0        0        0    15114 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/store.py
+-rw-r--r--   0        0        0     3746 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/task.py
+-rw-r--r--   0        0        0     6058 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/trigger.py
+-rw-r--r--   0        0        0     1892 2023-04-19 17:21:20.061974 motion_python-0.1.35/motion/utils.py
+-rw-r--r--   0        0        0     1578 2023-04-19 17:21:43.950314 motion_python-0.1.35/pyproject.toml
+-rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 motion_python-0.1.35/PKG-INFO
```

### Comparing `motion_python-0.1.34/README.md` & `motion_python-0.1.35/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/__init__.py` & `motion_python-0.1.35/motion/__init__.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/api/api.py` & `motion_python-0.1.35/motion/api/api.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/api/models.py` & `motion_python-0.1.35/motion/api/models.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/cli.py` & `motion_python-0.1.35/motion/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,24 +45,25 @@
     """Creates a new application."""
     motion.create_app(name, author)
 
     click.echo("Created a project successfully.")
 
 
 @motioncli.command("serve")
+@click.option("name", "--name", default="", help="Project name.")
 @click.option("host", "--host", default="0.0.0.0", help="Host to serve on.")
 @click.option("port", "--port", default=5000, help="Port to serve on.")
 @click.option(
     "logging_level",
     "--logging-level",
     "-l",
     default="WARNING",
     help="Logging level for motion. Can be DEBUG, INFO, WARNING, ERROR, CRITICAL.",
 )
-def serve(host: str, port: int, logging_level: str) -> None:
+def serve(name: str, host: str, port: int, logging_level: str) -> None:
     """Serves a Motion application."""
 
     # Check that the project is created
     if not os.path.exists("mconfig.py"):
         click.echo("Project is not created. Run `motion create` first.")
         return
 
@@ -73,14 +74,17 @@
 
     sys.path.append(os.getcwd())
 
     exec(config_code)
     mconfig = locals()["MCONFIG"]
     click.echo(f"Serving application {mconfig['application']['name']}...")
 
+    if name != "":
+        assert name == mconfig["application"]["name"], "Name does not match."
+
     # Serve the application
     motion.serve(mconfig, host=host, port=port, motion_logging_level=logging_level)
 
 
 @motioncli.command("clear")
 @click.argument("name", required=True)
 def clear(name: str) -> None:
```

### Comparing `motion_python-0.1.34/motion/client.py` & `motion_python-0.1.35/motion/client.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/cursor.py` & `motion_python-0.1.35/motion/cursor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 
 import collections
 import threading
 import typing
 import uuid
 from enum import Enum
+from typing import Any
 
 import duckdb
 import pandas as pd
 import pyarrow as pa
 import pyarrow.compute as pc
 
 from motion.utils import TriggerElement, TriggerFn, logger
@@ -469,17 +470,15 @@
         return self.mget(
             relation=relation,
             identifiers=all_ids,
             keys=keys,
             **kwargs,
         )
 
-    def _get_derived_ids(
-        self, con: duckdb.DuckDBPyConnection, identifier: str
-    ) -> list[str]:
+    def _get_derived_ids(self, con: duckdb.DuckDBPyConnection, identifier: str) -> Any:
         """Get all derived ids for an identifier.
 
         Args:
             con (duckdb.PyConnection): The connection to use.
             identifier (str): The identifier to get the derived ids for.
 
         Returns:
@@ -565,15 +564,15 @@
 
         res = res.to_pandas()
         if kwargs.get("as_df", False):
             return res
 
         return res.to_dict("records")
 
-    def getIdsForKey(self, relation: str, key: str, value: typing.Any) -> list[int]:
+    def getIdsForKey(self, relation: str, key: str, value: Any) -> Any:
         """Get ids for a key-value pair in a relation.
 
         Args:
             relation (str): The relation to get the value from.
             key (str): The key to get the values for.
             value (typing.Any): The value to get the ids for.
```

### Comparing `motion_python-0.1.34/motion/entry.py` & `motion_python-0.1.35/motion/entry.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/examples/cooking/dashboard.py` & `motion_python-0.1.35/motion/examples/cooking/dashboard.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/examples/cooking/test.py` & `motion_python-0.1.35/motion/examples/cooking/test.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/examples/cooking/triggers/scrape.py` & `motion_python-0.1.35/motion/examples/cooking/triggers/scrape.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/examples/cooking/triggers/search.py` & `motion_python-0.1.35/motion/examples/cooking/triggers/search.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/routing.py` & `motion_python-0.1.35/motion/routing.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/schema.py` & `motion_python-0.1.35/motion/schema.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/store.py` & `motion_python-0.1.35/motion/store.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/task.py` & `motion_python-0.1.35/motion/task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/trigger.py` & `motion_python-0.1.35/motion/trigger.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/motion/utils.py` & `motion_python-0.1.35/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.34/pyproject.toml` & `motion_python-0.1.35/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.34"
+version = "0.1.35"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 duckdb = "^0.7.1"
 click = "^8.1.3"
 colorlog = "^6.7.0"
 croniter = "^1.3.8"
 fastapi = "^0.95.0"
 pandas = "^1.5.3"
 pyarrow = "^11.0.0"
```

### Comparing `motion_python-0.1.34/PKG-INFO` & `motion_python-0.1.35/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.34
+Version: 0.1.35
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorlog (>=6.7.0,<7.0.0)
 Requires-Dist: croniter (>=1.3.8,<2.0.0)
 Requires-Dist: duckdb (>=0.7.1,<0.8.0)
```


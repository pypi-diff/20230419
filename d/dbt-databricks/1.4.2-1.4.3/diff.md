# Comparing `tmp/dbt-databricks-1.4.2.tar.gz` & `tmp/dbt-databricks-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-databricks-1.4.2.tar", last modified: Fri Feb 17 19:42:17 2023, max compression
+gzip compressed data, was "dbt-databricks-1.4.3.tar", last modified: Wed Apr 19 19:21:39 2023, max compression
```

## Comparing `dbt-databricks-1.4.2.tar` & `dbt-databricks-1.4.3.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-02-17 19:42:17.151184 dbt-databricks-1.4.2/
--rw-r--r--   0 andre.furlan   (502) staff       (20)       46 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/MANIFEST.in
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-02-17 19:42:17.150951 dbt-databricks-1.4.2/PKG-INFO
--rw-r--r--   0 andre.furlan   (502) staff       (20)     4572 2022-12-06 17:25:02.000000 dbt-databricks-1.4.2/README.md
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-02-17 19:42:17.133360 dbt-databricks-1.4.2/dbt/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-02-17 19:42:17.132942 dbt-databricks-1.4.2/dbt/adapters/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-02-17 19:42:17.141260 dbt-databricks-1.4.2/dbt/adapters/databricks/
--rw-r--r--   0 andre.furlan   (502) staff       (20)      626 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/dbt/adapters/databricks/__init__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)       23 2023-02-17 18:42:58.000000 dbt-databricks-1.4.2/dbt/adapters/databricks/__version__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)      586 2022-12-22 18:28:52.000000 dbt-databricks-1.4.2/dbt/adapters/databricks/column.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    21683 2023-01-31 00:57:55.000000 dbt-databricks-1.4.2/dbt/adapters/databricks/connections.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)    18978 2023-02-17 18:37:56.000000 dbt-databricks-1.4.2/dbt/adapters/databricks/impl.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2991 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/dbt/adapters/databricks/python_submissions.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2863 2023-02-01 01:31:07.000000 dbt-databricks-1.4.2/dbt/adapters/databricks/relation.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2117 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/dbt/adapters/databricks/utils.py
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-02-17 19:42:17.133516 dbt-databricks-1.4.2/dbt/include/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-02-17 19:42:17.142615 dbt-databricks-1.4.2/dbt/include/databricks/
--rw-r--r--   0 andre.furlan   (502) staff       (20)       52 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/dbt/include/databricks/__init__.py
--rw-r--r--   0 andre.furlan   (502) staff       (20)       77 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/dbt/include/databricks/dbt_project.yml
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-02-17 19:42:17.144250 dbt-databricks-1.4.2/dbt/include/databricks/macros/
--rw-r--r--   0 andre.furlan   (502) staff       (20)     8846 2022-12-22 18:28:52.000000 dbt-databricks-1.4.2/dbt/include/databricks/macros/adapters.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      592 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/dbt/include/databricks/macros/catalog.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2409 2023-01-31 00:57:55.000000 dbt-databricks-1.4.2/dbt/include/databricks/macros/copy_into.sql
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-02-17 19:42:17.145841 dbt-databricks-1.4.2/dbt/include/databricks/macros/materializations/
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-02-17 19:42:17.146788 dbt-databricks-1.4.2/dbt/include/databricks/macros/materializations/incremental/
--rw-r--r--   0 andre.furlan   (502) staff       (20)     4049 2022-12-22 18:28:52.000000 dbt-databricks-1.4.2/dbt/include/databricks/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      493 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/dbt/include/databricks/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2451 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/dbt/include/databricks/macros/materializations/seed.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5397 2022-12-06 17:25:02.000000 dbt-databricks-1.4.2/dbt/include/databricks/macros/materializations/snapshot.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)     1578 2022-12-06 17:25:02.000000 dbt-databricks-1.4.2/dbt/include/databricks/macros/materializations/table.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      119 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/dbt/include/databricks/macros/materializations/view.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      648 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/dbt/include/databricks/macros/statement.sql
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-02-17 19:42:17.147561 dbt-databricks-1.4.2/dbt/include/databricks/macros/utils/
--rw-r--r--   0 andre.furlan   (502) staff       (20)      318 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/dbt/include/databricks/macros/utils/dateadd.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      338 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/dbt/include/databricks/macros/utils/datediff.sql
--rw-r--r--   0 andre.furlan   (502) staff       (20)      475 2022-11-22 20:51:35.000000 dbt-databricks-1.4.2/dbt/include/databricks/profile_template.yml
-drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-02-17 19:42:17.150196 dbt-databricks-1.4.2/dbt_databricks.egg-info/
--rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-02-17 19:42:17.000000 dbt-databricks-1.4.2/dbt_databricks.egg-info/PKG-INFO
--rw-r--r--   0 andre.furlan   (502) staff       (20)     1317 2023-02-17 19:42:17.000000 dbt-databricks-1.4.2/dbt_databricks.egg-info/SOURCES.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-02-17 19:42:17.000000 dbt-databricks-1.4.2/dbt_databricks.egg-info/dependency_links.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-02-17 19:42:17.000000 dbt-databricks-1.4.2/dbt_databricks.egg-info/not-zip-safe
--rw-r--r--   0 andre.furlan   (502) staff       (20)       49 2023-02-17 19:42:17.000000 dbt-databricks-1.4.2/dbt_databricks.egg-info/requires.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)        4 2023-02-17 19:42:17.000000 dbt-databricks-1.4.2/dbt_databricks.egg-info/top_level.txt
--rw-r--r--   0 andre.furlan   (502) staff       (20)       38 2023-02-17 19:42:17.151248 dbt-databricks-1.4.2/setup.cfg
--rw-r--r--   0 andre.furlan   (502) staff       (20)     2538 2023-02-17 18:42:49.000000 dbt-databricks-1.4.2/setup.py
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.070120 dbt-databricks-1.4.3/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       46 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/MANIFEST.in
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-04-19 19:21:39.069902 dbt-databricks-1.4.3/PKG-INFO
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     4572 2023-04-19 17:50:57.000000 dbt-databricks-1.4.3/README.md
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.011645 dbt-databricks-1.4.3/dbt/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.011375 dbt-databricks-1.4.3/dbt/adapters/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.029839 dbt-databricks-1.4.3/dbt/adapters/databricks/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      626 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/__init__.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       23 2023-04-19 19:10:11.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/__version__.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      586 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/column.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    21683 2023-04-19 17:28:05.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/connections.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    19036 2023-04-19 17:59:40.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/impl.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)    17435 2023-04-19 17:59:31.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/python_submissions.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2863 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/relation.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2117 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/adapters/databricks/utils.py
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.012208 dbt-databricks-1.4.3/dbt/include/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.042760 dbt-databricks-1.4.3/dbt/include/databricks/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       52 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/dbt/include/databricks/__init__.py
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       77 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/dbt/include/databricks/dbt_project.yml
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.051440 dbt-databricks-1.4.3/dbt/include/databricks/macros/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     9909 2023-04-19 17:58:37.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/adapters.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      592 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/catalog.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2409 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/copy_into.sql
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.057181 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.062347 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/incremental/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     4128 2023-04-19 17:59:40.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     3910 2023-04-19 17:59:40.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2066 2023-04-19 17:59:40.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/incremental/validate.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2451 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/seed.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     5397 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/snapshot.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     1616 2023-04-19 17:58:37.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/table.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      119 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/view.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      648 2022-11-22 20:51:35.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/statement.sql
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.064714 dbt-databricks-1.4.3/dbt/include/databricks/macros/utils/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      318 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/utils/dateadd.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      338 2023-02-28 19:04:11.000000 dbt-databricks-1.4.3/dbt/include/databricks/macros/utils/datediff.sql
+-rw-r--r--   0 andre.furlan   (502) staff       (20)      475 2023-04-19 17:28:05.000000 dbt-databricks-1.4.3/dbt/include/databricks/profile_template.yml
+drwxr-xr-x   0 andre.furlan   (502) staff       (20)        0 2023-04-19 19:21:39.069428 dbt-databricks-1.4.3/dbt_databricks.egg-info/
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     5375 2023-04-19 19:21:38.000000 dbt-databricks-1.4.3/dbt_databricks.egg-info/PKG-INFO
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     1389 2023-04-19 19:21:39.000000 dbt-databricks-1.4.3/dbt_databricks.egg-info/SOURCES.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-04-19 19:21:38.000000 dbt-databricks-1.4.3/dbt_databricks.egg-info/dependency_links.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)        1 2023-02-17 19:42:17.000000 dbt-databricks-1.4.3/dbt_databricks.egg-info/not-zip-safe
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       49 2023-04-19 19:21:38.000000 dbt-databricks-1.4.3/dbt_databricks.egg-info/requires.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)        4 2023-04-19 19:21:38.000000 dbt-databricks-1.4.3/dbt_databricks.egg-info/top_level.txt
+-rw-r--r--   0 andre.furlan   (502) staff       (20)       38 2023-04-19 19:21:39.070174 dbt-databricks-1.4.3/setup.cfg
+-rw-r--r--   0 andre.furlan   (502) staff       (20)     2538 2023-04-19 17:59:55.000000 dbt-databricks-1.4.3/setup.py
```

### Comparing `dbt-databricks-1.4.2/PKG-INFO` & `dbt-databricks-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.4.2
+Version: 1.4.3
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.4.2/README.md` & `dbt-databricks-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.2/dbt/adapters/databricks/__init__.py` & `dbt-databricks-1.4.3/dbt/adapters/databricks/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.2/dbt/adapters/databricks/column.py` & `dbt-databricks-1.4.3/dbt/adapters/databricks/column.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.2/dbt/adapters/databricks/connections.py` & `dbt-databricks-1.4.3/dbt/adapters/databricks/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.2/dbt/adapters/databricks/impl.py` & `dbt-databricks-1.4.3/dbt/adapters/databricks/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,21 @@
     location_root: Optional[str] = None
     partition_by: Optional[Union[List[str], str]] = None
     clustered_by: Optional[Union[List[str], str]] = None
     buckets: Optional[int] = None
     options: Optional[Dict[str, str]] = None
     merge_update_columns: Optional[str] = None
     tblproperties: Optional[Dict[str, str]] = None
+    zorder: Optional[Union[List[str], str]] = None
+
+
+def check_not_found_error(errmsg: str) -> bool:
+    new_error = "[SCHEMA_NOT_FOUND]" in errmsg
+    old_error = re.match(r".*(Database).*(not found).*", errmsg, re.DOTALL)
+    return new_error or old_error is not None
 
 
 @undefined_proof
 class DatabricksAdapter(SparkAdapter):
 
     Relation = DatabricksRelation
     Column = DatabricksColumn
@@ -120,18 +127,15 @@
         self, schema_relation: DatabricksRelation
     ) -> List[DatabricksRelation]:
         kwargs = {"schema_relation": schema_relation}
         try:
             results = self.execute_macro(LIST_RELATIONS_MACRO_NAME, kwargs=kwargs)
         except dbt.exceptions.DbtRuntimeError as e:
             errmsg = getattr(e, "msg", "")
-            if (
-                "[SCHEMA_NOT_FOUND]" in errmsg
-                or f"Database '{schema_relation}' not found" in errmsg
-            ):
+            if check_not_found_error(errmsg):
                 return []
             else:
                 description = "Error while retrieving information about"
                 logger.debug(f"{description} {schema_relation}: {e.msg}")
                 raise e
 
         return [
@@ -152,18 +156,15 @@
         kwargs = {"schema_relation": schema_relation}
         try:
             # The catalog for `show table extended` needs to match the current catalog.
             with self._catalog(schema_relation.database):
                 results = self.execute_macro(SHOW_TABLE_EXTENDED_MACRO_NAME, kwargs=kwargs)
         except dbt.exceptions.DbtRuntimeError as e:
             errmsg = getattr(e, "msg", "")
-            if (
-                "[SCHEMA_NOT_FOUND]" in errmsg
-                or f"Database '{schema_relation.without_identifier()}' not found" in errmsg
-            ):
+            if check_not_found_error(errmsg):
                 results = []
             else:
                 description = "Error while retrieving information about"
                 logger.debug(f"{description} {schema_relation.without_identifier()}: {e.msg}")
                 raise e
 
         relations: List[Tuple[DatabricksRelation, str]] = []
@@ -446,15 +447,15 @@
             print(e)
             raise
         finally:
             cursor.close()
             conn.transaction_open = False
 
     def valid_incremental_strategies(self) -> List[str]:
-        return ["append", "merge", "insert_overwrite"]
+        return ["append", "merge", "insert_overwrite", "replace_where"]
 
     @property
     def python_submission_helpers(self) -> Dict[str, Type[PythonJobHelper]]:
         return {
             "job_cluster": DbtDatabricksJobClusterPythonJobHelper,
             "all_purpose_cluster": DbtDatabricksAllPurposeClusterPythonJobHelper,
         }
```

### Comparing `dbt-databricks-1.4.2/dbt/adapters/databricks/relation.py` & `dbt-databricks-1.4.3/dbt/adapters/databricks/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.2/dbt/adapters/databricks/utils.py` & `dbt-databricks-1.4.3/dbt/adapters/databricks/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.2/dbt/include/databricks/macros/adapters.sql` & `dbt-databricks-1.4.3/dbt/include/databricks/macros/adapters.sql`

 * *Files 4% similar despite different names*

```diff
@@ -107,14 +107,45 @@
 {% macro databricks__persist_constraints(relation, model) %}
   {% if config.get('persist_constraints', False) and config.get('file_format', 'delta') == 'delta' %}
     {% do alter_table_add_constraints(relation, model.meta.constraints) %}
     {% do alter_column_set_constraints(relation, model.columns) %}
   {% endif %}
 {% endmacro %}
 
+{% macro optimize(relation) %}
+  {{ return(adapter.dispatch('optimize', 'dbt')(relation)) }}
+{% endmacro %}
+
+{% macro databricks__optimize(relation) %}
+  {% if config.get('zorder', False) and config.get('file_format', 'delta') == 'delta' %}
+    {% if var('DATABRICKS_SKIP_OPTIMIZE', 'false')|lower != 'true' and var('databricks_skip_optimize', 'false')|lower != 'true' %}
+      {% call statement('run_optimize_stmt') %}
+        {{ get_optimize_sql(relation) }}
+      {% endcall %}
+    {% endif %}
+  {% endif %}
+{% endmacro %}
+
+{% macro get_optimize_sql(relation) %}
+  {% if config.get('zorder', False) and config.get('file_format', 'delta') == 'delta' %}
+     {%- set zorder = config.get('zorder', none) -%}
+    optimize {{ relation }}
+    {# TODO: predicates here? WHERE ...  #}
+    {% if zorder is sequence and zorder is not string %}
+      zorder by (
+        {%- for col in zorder -%}
+        {{ col }}{% if not loop.last %}, {% endif %}
+        {%- endfor -%}
+      )
+    {% else %}
+      zorder by ({{zorder}})
+    {% endif %}
+  {% endif %}
+{% endmacro %}
+
 {% macro alter_table_add_constraints(relation, constraints) %}
   {{ return(adapter.dispatch('alter_table_add_constraints', 'dbt')(relation, constraints)) }}
 {% endmacro %}
 
 {% macro databricks__alter_table_add_constraints(relation, constraints) %}
   {% if constraints is sequence %}
     {% for constraint in constraints %}
```

### Comparing `dbt-databricks-1.4.2/dbt/include/databricks/macros/catalog.sql` & `dbt-databricks-1.4.3/dbt/include/databricks/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.2/dbt/include/databricks/macros/copy_into.sql` & `dbt-databricks-1.4.3/dbt/include/databricks/macros/copy_into.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.2/dbt/include/databricks/macros/materializations/incremental/incremental.sql` & `dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/incremental/incremental.sql`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 {% materialization incremental, adapter='databricks', supported_languages=['sql', 'python'] -%}
   {#-- Validate early so we don't run SQL if the file_format + strategy combo is invalid --#}
   {%- set raw_file_format = config.get('file_format', default='delta') -%}
   {%- set raw_strategy = config.get('incremental_strategy') or 'merge' -%}
   {%- set grant_config = config.get('grants') -%}
 
-  {%- set file_format = dbt_spark_validate_get_file_format(raw_file_format) -%}
-  {%- set incremental_strategy = dbt_spark_validate_get_incremental_strategy(raw_strategy, file_format) -%}
+  {%- set file_format = dbt_databricks_validate_get_file_format(raw_file_format) -%}
+  {%- set incremental_strategy = dbt_databricks_validate_get_incremental_strategy(raw_strategy, file_format) -%}
 
   {#-- Set vars --#}
 
   {%- set incremental_predicates = config.get('predicates', default=none) or config.get('incremental_predicates', default=none) -%}
   {%- set unique_key = config.get('unique_key', none) -%}
   {%- set partition_by = config.get('partition_by', none) -%}
   {%- set language = model['language'] -%}
   {%- set on_schema_change = incremental_validate_on_schema_change(config.get('on_schema_change'), default='ignore') -%}
   {%- set target_relation = this -%}
   {%- set existing_relation = adapter.get_relation(database=this.database, schema=this.schema, identifier=this.identifier, needs_information=True) -%}
 
-  {#-- Set Overwrite Mode --#}
+  {#-- Set Overwrite Mode - does not work for warehouses --#}
   {%- if incremental_strategy == 'insert_overwrite' and partition_by -%}
     {%- call statement() -%}
       set spark.sql.sources.partitionOverwriteMode = DYNAMIC
     {%- endcall -%}
   {%- endif -%}
 
   {#-- Run pre-hooks --#}
@@ -78,12 +78,14 @@
   {% set should_revoke = should_revoke(existing_relation, full_refresh_mode) %}
   {% do apply_grants(target_relation, grant_config, should_revoke) %}
 
   {% do persist_docs(target_relation, model) %}
 
   {% do persist_constraints(target_relation, model) %}
 
+  {% do optimize(target_relation) %}
+
   {{ run_hooks(post_hooks) }}
 
   {{ return({'relations': [target_relation]}) }}
 
 {%- endmaterialization %}
```

### Comparing `dbt-databricks-1.4.2/dbt/include/databricks/macros/materializations/seed.sql` & `dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.2/dbt/include/databricks/macros/materializations/snapshot.sql` & `dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.2/dbt/include/databricks/macros/materializations/table.sql` & `dbt-databricks-1.4.3/dbt/include/databricks/macros/materializations/table.sql`

 * *Files 2% similar despite different names*

```diff
@@ -27,12 +27,14 @@
   {% set should_revoke = should_revoke(old_relation, full_refresh_mode=True) %}
   {% do apply_grants(target_relation, grant_config, should_revoke) %}
 
   {% do persist_docs(target_relation, model) %}
 
   {% do persist_constraints(target_relation, model) %}
 
+  {% do optimize(target_relation) %}
+
   {{ run_hooks(post_hooks) }}
 
   {{ return({'relations': [target_relation]})}}
 
 {% endmaterialization %}
```

### Comparing `dbt-databricks-1.4.2/dbt/include/databricks/macros/statement.sql` & `dbt-databricks-1.4.3/dbt/include/databricks/macros/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-databricks-1.4.2/dbt_databricks.egg-info/PKG-INFO` & `dbt-databricks-1.4.3/dbt_databricks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-databricks
-Version: 1.4.2
+Version: 1.4.3
 Summary: The Databricks adapter plugin for dbt
 Home-page: https://github.com/databricks/dbt-databricks
 Author: Databricks
 Author-email: feedback@databricks.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `dbt-databricks-1.4.2/dbt_databricks.egg-info/SOURCES.txt` & `dbt-databricks-1.4.3/dbt_databricks.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 dbt/include/databricks/macros/statement.sql
 dbt/include/databricks/macros/materializations/seed.sql
 dbt/include/databricks/macros/materializations/snapshot.sql
 dbt/include/databricks/macros/materializations/table.sql
 dbt/include/databricks/macros/materializations/view.sql
 dbt/include/databricks/macros/materializations/incremental/incremental.sql
 dbt/include/databricks/macros/materializations/incremental/strategies.sql
+dbt/include/databricks/macros/materializations/incremental/validate.sql
 dbt/include/databricks/macros/utils/dateadd.sql
 dbt/include/databricks/macros/utils/datediff.sql
 dbt_databricks.egg-info/PKG-INFO
 dbt_databricks.egg-info/SOURCES.txt
 dbt_databricks.egg-info/dependency_links.txt
 dbt_databricks.egg-info/not-zip-safe
 dbt_databricks.egg-info/requires.txt
```

### Comparing `dbt-databricks-1.4.2/setup.py` & `dbt-databricks-1.4.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     author="Databricks",
     author_email="feedback@databricks.com",
     url="https://github.com/databricks/dbt-databricks",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
         "dbt-spark~={}".format(dbt_spark_version),
-        "databricks-sql-connector>=2.2.2",
+        "databricks-sql-connector>=2.5.0",
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS :: MacOS X",
```


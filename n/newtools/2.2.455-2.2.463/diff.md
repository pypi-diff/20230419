# Comparing `tmp/newtools-2.2.455.tar.gz` & `tmp/newtools-2.2.463.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/newtools-2.2.455.tar", last modified: Wed Apr  5 12:35:27 2023, max compression
+gzip compressed data, was "dist/newtools-2.2.463.tar", last modified: Wed Apr 19 13:33:43 2023, max compression
```

## Comparing `newtools-2.2.455.tar` & `newtools-2.2.463.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-05 12:35:27.000000 newtools-2.2.455/
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-05 12:33:36.000000 newtools-2.2.455/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-05 12:35:27.000000 newtools-2.2.455/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-05 12:33:36.000000 newtools-2.2.455/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-05 12:35:27.000000 newtools-2.2.455/newtools/
--rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-05 12:35:27.000000 newtools-2.2.455/newtools/aws/
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/aws/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9641 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/aws/load_partitions.py
--rw-rw-rw-   0 root         (0) root         (0)     6435 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/aws/s3_location.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-05 12:35:27.000000 newtools-2.2.455/newtools/db/
--rw-rw-rw-   0 root         (0) root         (0)      285 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6912 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/db/athena.py
--rw-rw-rw-   0 root         (0) root         (0)    36570 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/db/cached_query.py
--rw-rw-rw-   0 root         (0) root         (0)    12954 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/db/sql_client.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-05 12:35:27.000000 newtools-2.2.455/newtools/doggo/
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/doggo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5576 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/doggo/csv.py
--rw-rw-rw-   0 root         (0) root         (0)    13397 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/doggo/doggo.py
--rw-rw-rw-   0 root         (0) root         (0)    19227 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/doggo/fs.py
--rw-rw-rw-   0 root         (0) root         (0)     9277 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/doggo/lock.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-05 12:35:27.000000 newtools-2.2.455/newtools/log/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/log/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9531 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/log/json_persistent_field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3858 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/log/log.py
--rw-rw-rw-   0 root         (0) root         (0)     2931 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/log/persistent_field_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3452 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/optional_imports.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-05 12:35:27.000000 newtools-2.2.455/newtools/queue/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/queue/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5151 2023-04-05 12:33:36.000000 newtools-2.2.455/newtools/queue/task_queue.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-05 12:35:27.000000 newtools-2.2.455/newtools.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-05 12:35:27.000000 newtools-2.2.455/newtools.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      797 2023-04-05 12:35:27.000000 newtools-2.2.455/newtools.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-05 12:35:27.000000 newtools-2.2.455/newtools.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-05 12:35:27.000000 newtools-2.2.455/newtools.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      119 2023-04-05 12:35:27.000000 newtools-2.2.455/newtools.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-05 12:35:27.000000 newtools-2.2.455/newtools.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-05 12:33:36.000000 newtools-2.2.455/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-05 12:35:27.000000 newtools-2.2.455/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     2296 2023-04-05 12:33:36.000000 newtools-2.2.455/setup.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-05 12:35:24.000000 newtools-2.2.455/version.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/
+-rw-rw-rw-   0 root         (0) root         (0)       62 2023-04-19 13:31:44.000000 newtools-2.2.463/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-19 13:33:43.000000 newtools-2.2.463/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-19 13:31:44.000000 newtools-2.2.463/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools/
+-rw-rw-rw-   0 root         (0) root         (0)      648 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools/aws/
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/aws/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9641 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/aws/load_partitions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6435 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/aws/s3_location.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools/db/
+-rw-rw-rw-   0 root         (0) root         (0)      285 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6912 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/db/athena.py
+-rw-rw-rw-   0 root         (0) root         (0)    39426 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/db/cached_query.py
+-rw-rw-rw-   0 root         (0) root         (0)    12954 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/db/sql_client.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools/doggo/
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/doggo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5576 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/doggo/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    13397 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/doggo/doggo.py
+-rw-rw-rw-   0 root         (0) root         (0)    19227 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/doggo/fs.py
+-rw-rw-rw-   0 root         (0) root         (0)     9277 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/doggo/lock.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools/log/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/log/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9531 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/log/json_persistent_field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3858 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/log/log.py
+-rw-rw-rw-   0 root         (0) root         (0)     2931 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/log/persistent_field_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3452 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/optional_imports.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools/queue/
+-rw-rw-rw-   0 root         (0) root         (0)       72 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/queue/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5151 2023-04-19 13:31:44.000000 newtools-2.2.463/newtools/queue/task_queue.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     1305 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      797 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      119 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-04-19 13:33:43.000000 newtools-2.2.463/newtools.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-04-19 13:31:45.000000 newtools-2.2.463/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      252 2023-04-19 13:33:43.000000 newtools-2.2.463/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     2296 2023-04-19 13:31:45.000000 newtools-2.2.463/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-04-19 13:33:37.000000 newtools-2.2.463/version.txt
```

### Comparing `newtools-2.2.455/PKG-INFO` & `newtools-2.2.463/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtools
-Version: 2.2.455
+Version: 2.2.463
 Summary: Provides useful libraries for processing large data sets.
 Home-page: https://bitbucket.org/deductive/newtools/
 Author: Deductive
 Author-email: hello@deductive.com
 License: MIT
 Project-URL: Documentation, https://newtools.readthedocs.io/en/latest/
 Project-URL: Source, https://bitbucket.org/deductive/newtools/
```

### Comparing `newtools-2.2.455/README.md` & `newtools-2.2.463/README.md`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/__init__.py` & `newtools-2.2.463/newtools/__init__.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/aws/load_partitions.py` & `newtools-2.2.463/newtools/aws/load_partitions.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/aws/s3_location.py` & `newtools-2.2.463/newtools/aws/s3_location.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/db/athena.py` & `newtools-2.2.463/newtools/db/athena.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/db/cached_query.py` & `newtools-2.2.463/newtools/db/cached_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -752,34 +752,42 @@
         cache_path: Optional[Path] = '',
         sql_archive_path: Optional[str] = None,
         sql_paths: Optional[Union[str, List[str]]] = None,
         dynamodb_lock: Optional[bool] = True,
         use_lock: Optional[bool] = True,
         logger: Optional[logging.Logger] = logging.getLogger(__name__),
         expiry_seconds: Optional[int] = 0,
-        queue_queries: Optional[bool] = False
+        queue_queries: Optional[bool] = False,
+        return_meta: Optional[bool] = False
     ) -> None:
         """
         :param use_lock: whether to use a lock to prevent concurrent s3 access
             if set to False, dynamodb_lock parameter wll be ignored
+        :param return_meta: whether to return the metadata of the query (e.g. count(1) of the results)
+            this functionality will only work if queue_queries is set to False
         """
         if cache_path and not cache_path.startswith('s3://'):
             raise AssertionError(f"CTAS queries can only output to S3; current cache path: {cache_path}")
 
+        self.query_meta = {}
+
         super().__init__(
             params=params,
             cache_path=cache_path,
             sql_archive_path=sql_archive_path,
             sql_paths=sql_paths,
             dynamodb_lock=dynamodb_lock,
             logger=logger,
             expiry_seconds=expiry_seconds,
             use_lock=use_lock
         )
+
+        self.return_meta = return_meta
         self.queue_queries = queue_queries
+
         self.doggo = PandasDoggo()
 
     @classmethod
     def get_query_header(
         cls,
         database: str,
         table_name: str,
@@ -832,27 +840,39 @@
         self,
         sql_file: str,
         output_prefix: str,
         params: Optional[dict] = None,
         replacement_dict: Optional[dict] = None,
         refresh_cache: Optional[bool] = False,
         **kwargs
-    ) -> str:
+    ) -> Union[str, dict]:
         """
         Function to run the specified query and return the output path(/directory) to the data.
+        If return_meta is set to True, will return a dictionary containing the output path and the metadata.
+        The query metadata is refreshed on get_results() call.
         """
-        return super().get_results(
+        self.query_meta = {}
+
+        output_path = super().get_results(
             sql_file=sql_file,
             output_prefix=output_prefix,
             params=params,
             replacement_dict=replacement_dict,
             refresh_cache=refresh_cache,
             ignore_list=['partition_columns']
         )
 
+        if self.return_meta:
+            return {
+                'output_path': output_path,
+                **self.query_meta
+            }
+        else:
+            return output_path
+
     @staticmethod
     def get_cache_file_format(*args, **kwargs) -> str:
         """
         Return the file format for the cache path for CTAS.
         """
         return "/"
 
@@ -885,14 +905,21 @@
             name="CTAS {}".format(output_file),
             output_location=self.cache_path
         )
 
         if not self.queue_queries:
             self._ac.wait_for_completion()
 
+            if self.return_meta:
+                self.get_query_metadata(
+                    database=ctas_params.get('database'),
+                    table_name=ctas_params.get('table_name'),
+                    partition_columns=ctas_params.get('partition_columns')
+                )
+
             # If CTAS has no results, no files are saved to S3 - so we do so for caching purposes
             if not self.dfs.exists(output_file):
                 self.dfs.s3_client.put_object(
                     Bucket=S3Location(output_file).bucket,
                     Key=S3Location(output_file).join('EMPTY').key,
                     Body=b''
                 )
@@ -901,14 +928,65 @@
             self._ac.add_query(
                 sql=f"DROP TABLE IF EXISTS {ctas_params['database']}.{ctas_params['table_name']}",
                 name="DROP CTAS {}".format(output_file),
                 output_location=self.cache_path
             )
             self._ac.wait_for_completion()
 
+    def get_query_metadata(
+        self,
+        database: str,
+        table_name: str,
+        partition_columns: Optional[Union[str, list]] = None
+    ) -> None:
+        """
+        Function to run queries to get metadata about the results of the query from CTAS.
+
+        :param database: the database the table is stored in
+        :param table_name: the name of the CTAS table
+        :param partition_columns: the partitions columns used in the query (if any)
+        """
+        base_query = """SELECT {columns} COUNT(1) FROM {database}.{table_name} {group_by}"""
+        columns = group_by = ""
+
+        if partition_columns:
+            partition_columns = partition_columns if isinstance(partition_columns, list) else [partition_columns]
+            columns = ", ".join(partition_columns) + ","
+            group_by = f"GROUP BY {', '.join(str(i) for i in range(1, len(partition_columns) + 1))}"
+
+        query = base_query.format(
+            columns=columns,
+            database=database,
+            table_name=table_name,
+            group_by=group_by
+        )
+
+        query_id = self._ac.add_query(query, output_location=self.cache_path)
+        self._ac.wait_for_completion()
+        results = self._ac.get_query_result(query_id)
+
+        self.query_meta['size'] = self.format_df_to_dict(results, index_cols=partition_columns)
+
+    @staticmethod
+    def format_df_to_dict(
+        df: DataFrame,
+        index_cols: Optional[List[str]] = None
+    ) -> dict:
+        """
+        Function to format a dataframe into a dictionary of values.
+
+        :param df: the dataframe to format
+        :param index_cols: the columns to set as the index
+        """
+        col_name = df.columns[-1]
+        if index_cols:
+            return df.set_index(index_cols).to_dict()[col_name]
+        else:
+            return {'total': df.loc[0, col_name]}
+
     @staticmethod
     def validate_ctas_params(
         parameters: dict
     ) -> None:
         """
         Function to check the required parameters for CTAS are specified in the parameters.
         """
```

### Comparing `newtools-2.2.455/newtools/db/sql_client.py` & `newtools-2.2.463/newtools/db/sql_client.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/doggo/csv.py` & `newtools-2.2.463/newtools/doggo/csv.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/doggo/doggo.py` & `newtools-2.2.463/newtools/doggo/doggo.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/doggo/fs.py` & `newtools-2.2.463/newtools/doggo/fs.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/doggo/lock.py` & `newtools-2.2.463/newtools/doggo/lock.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/log/json_persistent_field_logger.py` & `newtools-2.2.463/newtools/log/json_persistent_field_logger.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/log/log.py` & `newtools-2.2.463/newtools/log/log.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/log/persistent_field_logger.py` & `newtools-2.2.463/newtools/log/persistent_field_logger.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/optional_imports.py` & `newtools-2.2.463/newtools/optional_imports.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools/queue/task_queue.py` & `newtools-2.2.463/newtools/queue/task_queue.py`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/newtools.egg-info/PKG-INFO` & `newtools-2.2.463/newtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: newtools
-Version: 2.2.455
+Version: 2.2.463
 Summary: Provides useful libraries for processing large data sets.
 Home-page: https://bitbucket.org/deductive/newtools/
 Author: Deductive
 Author-email: hello@deductive.com
 License: MIT
 Project-URL: Documentation, https://newtools.readthedocs.io/en/latest/
 Project-URL: Source, https://bitbucket.org/deductive/newtools/
```

### Comparing `newtools-2.2.455/newtools.egg-info/SOURCES.txt` & `newtools-2.2.463/newtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `newtools-2.2.455/setup.py` & `newtools-2.2.463/setup.py`

 * *Files identical despite different names*


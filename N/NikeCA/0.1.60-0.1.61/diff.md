# Comparing `tmp/NikeCA-0.1.60.tar.gz` & `tmp/NikeCA-0.1.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikeCA-0.1.60.tar", last modified: Mon Apr 17 21:05:43 2023, max compression
+gzip compressed data, was "NikeCA-0.1.61.tar", last modified: Wed Apr 19 04:47:22 2023, max compression
```

## Comparing `NikeCA-0.1.60.tar` & `NikeCA-0.1.61.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 21:05:43.621739 NikeCA-0.1.60/
--rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.60/LICENSE
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 21:05:43.621428 NikeCA-0.1.60/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.60/README.md
--rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-17 21:05:43.621819 NikeCA-0.1.60/setup.cfg
--rw-r--r--   0 WCheaq     (502) staff       (20)     2270 2023-04-17 21:05:16.000000 NikeCA-0.1.60/setup.py
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 21:05:43.619090 NikeCA-0.1.60/src/
-drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-17 21:05:43.620819 NikeCA-0.1.60/src/NikeCA.egg-info/
--rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-17 21:05:43.000000 NikeCA-0.1.60/src/NikeCA.egg-info/PKG-INFO
--rw-r--r--   0 WCheaq     (502) staff       (20)      444 2023-04-17 21:05:43.000000 NikeCA-0.1.60/src/NikeCA.egg-info/SOURCES.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-17 21:05:43.000000 NikeCA-0.1.60/src/NikeCA.egg-info/dependency_links.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-17 21:05:43.000000 NikeCA-0.1.60/src/NikeCA.egg-info/requires.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)      158 2023-04-17 21:05:43.000000 NikeCA-0.1.60/src/NikeCA.egg-info/top_level.txt
--rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/NikeCA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/NikeQA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    21686 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/NikeSF.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_BuildSearchQuery.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3744 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_Dashboards.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_GitHub.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     4071 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_InclusionExclusion.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_QA.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_SearchFiles.py
--rw-r--r--   0 WCheaq     (502) staff       (20)    14098 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_SnowflakeData.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_SnowflakeDependencies.py
--rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/_SnowflakePull.py
--rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-17 21:04:59.000000 NikeCA-0.1.60/src/__init__.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-19 04:47:22.296089 NikeCA-0.1.61/
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1069 2023-02-18 07:46:56.000000 NikeCA-0.1.61/LICENSE
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-19 04:47:22.295635 NikeCA-0.1.61/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17621 2023-03-15 23:26:31.000000 NikeCA-0.1.61/README.md
+-rw-r--r--   0 WCheaq     (502) staff       (20)       38 2023-04-19 04:47:22.296213 NikeCA-0.1.61/setup.cfg
+-rw-r--r--   0 WCheaq     (502) staff       (20)     2270 2023-04-19 04:47:00.000000 NikeCA-0.1.61/setup.py
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-19 04:47:22.290492 NikeCA-0.1.61/src/
+drwxr-xr-x   0 WCheaq     (502) staff       (20)        0 2023-04-19 04:47:22.292812 NikeCA-0.1.61/src/NikeCA.egg-info/
+-rw-r--r--   0 WCheaq     (502) staff       (20)    18047 2023-04-19 04:47:22.000000 NikeCA-0.1.61/src/NikeCA.egg-info/PKG-INFO
+-rw-r--r--   0 WCheaq     (502) staff       (20)      444 2023-04-19 04:47:22.000000 NikeCA-0.1.61/src/NikeCA.egg-info/SOURCES.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)        1 2023-04-19 04:47:22.000000 NikeCA-0.1.61/src/NikeCA.egg-info/dependency_links.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)     1155 2023-04-19 04:47:22.000000 NikeCA-0.1.61/src/NikeCA.egg-info/requires.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)      158 2023-04-19 04:47:22.000000 NikeCA-0.1.61/src/NikeCA.egg-info/top_level.txt
+-rw-r--r--   0 WCheaq     (502) staff       (20)       92 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/NikeCA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14406 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/NikeQA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    23489 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/NikeSF.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     4372 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_BuildSearchQuery.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3744 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_Dashboards.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    13607 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_GitHub.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     9037 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_InclusionExclusion.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    17212 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_QA.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     3546 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_SearchFiles.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)    14098 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_SnowflakeData.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7062 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_SnowflakeDependencies.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)     7114 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/_SnowflakePull.py
+-rw-r--r--   0 WCheaq     (502) staff       (20)        0 2023-04-19 04:45:37.000000 NikeCA-0.1.61/src/__init__.py
```

### Comparing `NikeCA-0.1.60/LICENSE` & `NikeCA-0.1.61/LICENSE`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.60/PKG-INFO` & `NikeCA-0.1.61/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.60
+Version: 0.1.61
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.60/README.md` & `NikeCA-0.1.61/README.md`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.60/setup.py` & `NikeCA-0.1.61/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
 	long_description = fh.read()
 
 
 setup(
 	name='NikeCA',
-	version='0.1.60',
+	version='0.1.61',
 	description='Standardize and Automate processes utilized by the DAMs at Nike in CA',
 	py_modules=[
 		"__init__",
 		"NikeSF",
 		"_SnowflakeData",
 		"_BuildSearchQuery",
 		"_Dashboards",
```

### Comparing `NikeCA-0.1.60/src/NikeCA.egg-info/PKG-INFO` & `NikeCA-0.1.61/src/NikeCA.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikeCA
-Version: 0.1.60
+Version: 0.1.61
 Summary: Standardize and Automate processes utilized by the DAMs at Nike in CA
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `NikeCA-0.1.60/src/NikeCA.egg-info/requires.txt` & `NikeCA-0.1.61/src/NikeCA.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.60/src/NikeQA.py` & `NikeCA-0.1.61/src/NikeQA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.60/src/NikeSF.py` & `NikeCA-0.1.61/src/NikeSF.py`

 * *Files 3% similar despite different names*

```diff
@@ -231,16 +231,22 @@
     def polars(self):
         return self.__polars
 
     @polars.setter
     def polars(self, value):
         self.__polars = value
 
-    def build_search_query(self, inp_db: str = None, schema: str = None, table: str = None,
-                           column_name=None, like_flag: bool = False, col_and_or: str = 'AND'):
+    def build_search_query(self
+                           , inp_db: str = None
+                           , schema: str = None
+                           , table: str = None
+                           , column_name=None
+                           , like_flag: bool = False
+                           , col_and_or: str = 'AND'
+                           ):
         """
         Builds and returns a search query based on the specified parameters and instance variables.
 
         Parameters:
             inp_db (str or None, optional): The database to use (default is None).
             schema (str or None, optional): The schema to use (default is None).
             table (str or None, optional): The table to search (default is None).
@@ -273,15 +279,16 @@
                        schema: str = None,
                        table: str = None,
                        sample_table: bool = False,
                        sample_val: bool = False,
                        table_sample: dict = None,
                        dtypes_conv=None,
                        separate_dataframes: bool = True,
-                       polars: bool = False):
+                       polars: bool = False
+                       ):
 
         """
         Executes a query in Snowflake and returns the results as a Pandas DataFrame.
 
         Parameters:
             query (str): The SQL query to execute.
             username (str, optional): The Snowflake username to use. If not provided, uses the one set in the class
@@ -357,15 +364,16 @@
                       table_sample: dict = None,
                       dtypes_conv=None,
                       schema: str = None,
                       table: str = None,
                       column_name: str = None,
                       col_and_or='and',
                       get_ex_val: bool = False,
-                      like_flag: bool = False) -> pd.DataFrame:
+                      like_flag: bool = False
+                      ) -> pd.DataFrame:
 
         """
         search snowflake structure for specific schema/table/column;
         (optional) specify to return example values from each table-column
 
         :param username: Any = None
         :param warehouse: Any = None
@@ -425,15 +433,16 @@
                          warehouse: str | None = None,
                          role: str | None = None,
                          database: str | None = None,
                          schema: str | None = None,
                          table_name: str | None = None,
                          pull_all_cols: bool = True,
                          run_debugging: bool = False,
-                         query: any = None):
+                         query: any = None
+                         ):
 
         """
         build a dictionary containing keys that reference column:datatype conversion
         (w/ the purpose of optimizing memory after pulling data)
 
         :param username: str or None = None
         :param warehouse: str or None = None
@@ -453,26 +462,26 @@
             warehouse = self.__warehouse
         if role is None:
             role = self.__role
         if database is None:
             database = self.__database
 
         return SnowflakeData.optimize_tbl_mem(self, username=username, warehouse=warehouse, role=role,
-                                                             database=database, schema=schema, table_name=table_name,
-                                                             pull_all_cols=pull_all_cols, run_debugging=run_debugging,
-                                                             query=query)
+                                              database=database, schema=schema, table_name=table_name,
+                                              pull_all_cols=pull_all_cols, run_debugging=run_debugging, query=query)
 
     def snowflake_dependencies(self,
                                tables: str | list | None = None,
                                username: str | None = None,
                                warehouse: str | None = None,
                                role: str | None = None,
                                database: str | None = None,
                                schema: str | list | None = None,
-                               save_path: str = None):
+                               save_path: str = None
+                               ):
 
         """
 
         :param save_path:
         :param tables:
         :param username:
         :param warehouse:
@@ -505,15 +514,16 @@
                               , username: str | None = None
                               , warehouse: str | None = None
                               , database: str | None = None
                               , role: str | None = None
                               , date_min: str = '1900-01-01'
                               , date_max: str = '9999-12-31'
                               , column_filters=None
-                              , polars: bool = False):
+                              , polars: bool = False
+                              ):
 
         if username is None:
             username = self.__username
         if warehouse is None:
             warehouse = self.__warehouse
         if database is None:
             database = self.__database
@@ -536,48 +546,84 @@
                                 , username: str = None
                                 , warehouse: str = None
                                 , database: str = None
                                 , role: str = None
                                 , columns=None
                                 , filters=None
                                 , order_by=None
-                                , polars: bool = False):
+                                , polars: bool = False
+                                , start_date: str | None = None
+                                , end_date: str | None = None
+                                ):
 
         if username is None:
             username = self.__username
         if warehouse is None:
             warehouse = self.__warehouse
         if database is None:
             database = self.__database
         if role is None:
             role = self.__role
         if polars is False:
             polars = self.__polars
 
         return InclusionExclusion.pos_data_quality_review(self, username=username, warehouse=warehouse,
                                                           database=database, role=role, columns=columns,
-                                                          filters=filters, order_by=order_by, polars=polars)
+                                                          filters=filters, order_by=order_by, polars=polars,
+                                                          start_date=start_date, end_date=end_date)
 
     def summary(self
                 , username: str = None
                 , warehouse: str = None
                 , database: str = None
                 , role: str = None
                 , columns=None
                 , filters=None
                 , order_by=None
-                , polars: bool = True):
+                , polars: bool = True
+                , start_date: str | None = None
+                , end_date: str | None = None
+                ):
 
         if username is None:
             username = self.__username
         if warehouse is None:
             warehouse = self.__warehouse
         if database is None:
             database = self.__database
         if role is None:
             role = self.__role
         if polars is False:
             polars = self.__polars
 
         return InclusionExclusion.summary(self, username=username, warehouse=warehouse, database=database, role=role,
-                                          columns=columns, filters=filters, order_by=order_by, polars=polars)
+                                          columns=columns, filters=filters, order_by=order_by, polars=polars,
+                                          start_date=start_date, end_date=end_date)
+
+    def home_summary(self
+                     , username: str = None
+                     , warehouse: str = None
+                     , database: str = None
+                     , role: str = None
+                     , columns=None
+                     , filters=None
+                     , order_by=None
+                     , polars: bool = True
+                     , start_date: str | None = None
+                     , end_date: str | None = None
+                     ):
+
+        if username is None:
+            username = self.__username
+        if warehouse is None:
+            warehouse = self.__warehouse
+        if database is None:
+            database = self.__database
+        if role is None:
+            role = self.__role
+        if polars is False:
+            polars = self.__polars
+
+        return InclusionExclusion.home_summary(self, username=username, warehouse=warehouse, database=database,
+                                               role=role, columns=columns, filters=filters, order_by=order_by,
+                                               polars=polars, start_date=start_date, end_date=end_date)
```

### Comparing `NikeCA-0.1.60/src/_BuildSearchQuery.py` & `NikeCA-0.1.61/src/_BuildSearchQuery.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.60/src/_Dashboards.py` & `NikeCA-0.1.61/src/_Dashboards.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.60/src/_GitHub.py` & `NikeCA-0.1.61/src/_GitHub.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.60/src/_QA.py` & `NikeCA-0.1.61/src/_QA.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.60/src/_SearchFiles.py` & `NikeCA-0.1.61/src/_SearchFiles.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.60/src/_SnowflakeData.py` & `NikeCA-0.1.61/src/_SnowflakeData.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.60/src/_SnowflakeDependencies.py` & `NikeCA-0.1.61/src/_SnowflakeDependencies.py`

 * *Files identical despite different names*

### Comparing `NikeCA-0.1.60/src/_SnowflakePull.py` & `NikeCA-0.1.61/src/_SnowflakePull.py`

 * *Files identical despite different names*


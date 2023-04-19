# Comparing `tmp/etl_csm_pet-0.0.3.tar.gz` & `tmp/etl_csm_pet-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_csm_pet-0.0.3.tar", last modified: Fri Apr 14 17:03:01 2023, max compression
+gzip compressed data, was "etl_csm_pet-0.0.4.tar", last modified: Wed Apr 19 17:44:04 2023, max compression
```

## Comparing `etl_csm_pet-0.0.3.tar` & `etl_csm_pet-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 17:03:01.846418 etl_csm_pet-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-04-14 17:03:01.841418 etl_csm_pet-0.0.3/Etl/
--rw-rw-rw-   0        0        0     3381 2023-04-14 13:56:04.000000 etl_csm_pet-0.0.3/Etl/Execute.py
--rw-rw-rw-   0        0        0     1547 2023-04-14 15:13:09.000000 etl_csm_pet-0.0.3/Etl/Extrator.py
--rw-rw-rw-   0        0        0     1965 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.3/Etl/Helper.py
--rw-rw-rw-   0        0        0     1761 2023-04-14 15:13:16.000000 etl_csm_pet-0.0.3/Etl/Loader.py
--rw-rw-rw-   0        0        0     4814 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.3/Etl/Treatment_extras.py
--rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm_pet-0.0.3/Etl/Treatment_tracking.py
--rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.3/Etl/Treatment_tracking_pme.py
--rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.3/Etl/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm_pet-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      552 2023-04-14 17:03:01.845419 etl_csm_pet-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm_pet-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-14 17:03:01.845419 etl_csm_pet-0.0.3/etl_csm_pet.egg-info/
--rw-rw-rw-   0        0        0      552 2023-04-14 17:03:01.000000 etl_csm_pet-0.0.3/etl_csm_pet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-04-14 17:03:01.000000 etl_csm_pet-0.0.3/etl_csm_pet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-14 17:03:01.000000 etl_csm_pet-0.0.3/etl_csm_pet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-14 17:03:01.000000 etl_csm_pet-0.0.3/etl_csm_pet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-14 17:03:01.000000 etl_csm_pet-0.0.3/etl_csm_pet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-14 17:03:01.846418 etl_csm_pet-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-04-14 17:02:43.000000 etl_csm_pet-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:44:04.165247 etl_csm_pet-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-04-19 17:44:04.160245 etl_csm_pet-0.0.4/Etl/
+-rw-rw-rw-   0        0        0     3381 2023-04-19 17:00:12.000000 etl_csm_pet-0.0.4/Etl/Execute.py
+-rw-rw-rw-   0        0        0     1577 2023-04-19 17:00:12.000000 etl_csm_pet-0.0.4/Etl/Extrator.py
+-rw-rw-rw-   0        0        0     2794 2023-04-19 17:33:43.000000 etl_csm_pet-0.0.4/Etl/Helper.py
+-rw-rw-rw-   0        0        0     1978 2023-04-19 17:19:57.000000 etl_csm_pet-0.0.4/Etl/Loader.py
+-rw-rw-rw-   0        0        0     4814 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.4/Etl/Treatment_extras.py
+-rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm_pet-0.0.4/Etl/Treatment_tracking.py
+-rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.4/Etl/Treatment_tracking_pme.py
+-rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.4/Etl/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm_pet-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      552 2023-04-19 17:44:04.164245 etl_csm_pet-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm_pet-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 17:44:04.164245 etl_csm_pet-0.0.4/etl_csm_pet.egg-info/
+-rw-rw-rw-   0        0        0      552 2023-04-19 17:44:03.000000 etl_csm_pet-0.0.4/etl_csm_pet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-04-19 17:44:03.000000 etl_csm_pet-0.0.4/etl_csm_pet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 17:44:03.000000 etl_csm_pet-0.0.4/etl_csm_pet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-19 17:44:03.000000 etl_csm_pet-0.0.4/etl_csm_pet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-19 17:44:03.000000 etl_csm_pet-0.0.4/etl_csm_pet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 17:44:04.165247 etl_csm_pet-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-04-19 17:43:23.000000 etl_csm_pet-0.0.4/setup.py
```

### Comparing `etl_csm_pet-0.0.3/Etl/Execute.py` & `etl_csm_pet-0.0.4/Etl/Execute.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.3/Etl/Extrator.py` & `etl_csm_pet-0.0.4/Etl/Extrator.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,9 +46,10 @@
         df = Dataframe base
     """
     new_df = pd.DataFrame(list(df['global_extras_raw']))
     if new_df.empty:
         raise Exception('O seu dataframe de extras está vazio! Verifique o seu query')
     return new_df
 
-
+def expurge_to_s3():
+    pass
```

### Comparing `etl_csm_pet-0.0.3/Etl/Helper.py` & `etl_csm_pet-0.0.4/Etl/Helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sqlalchemy
 from typing import Type
 from functools import wraps
 from time import time
 from logging import info
 from io import StringIO
 from csv import writer
 from numpy import nan
@@ -45,19 +46,41 @@
             table_name = '{}.{}'.format(table.schema, table.name)
         else:
             table_name = table.name
         sql = 'COPY {} ({}) FROM STDIN WITH CSV'.format(
             table_name, columns)
         cur.copy_expert(sql=sql, file=s_buf)
 
-def map_substring(s, dict_map):
+def map_substring(s, dict_map) -> dict:
     """
     Funcao helper mapeia as sub strings com facilidade
     ARGS
     s = pd.Series a ser interada por
     dict_map = mapa se substrings
     
     """
     for key in dict_map.keys():
         if key in s: 
             return dict_map[key]
-    return nan
+    return nan
+
+def sqlcol(df) -> dict:
+    """
+    
+    Funcao que mapeia os datatype das tabelas e retorna o datatype adequado do SQLalchemy
+    ARGS
+    df, para acessar os objetos de colunas e datatypes
+    """
+    info("Formulando dict_map de datatype SQLalchemy")
+    dtypedict = {}
+    for i,j in zip(df.columns, df.dtypes):
+        if "object" in str(j):
+            dtypedict.update({i: sqlalchemy.types.VARCHAR(length=300)})                 
+        if "datetime" in str(j):
+            dtypedict.update({i: sqlalchemy.types.DateTime()})
+        if "float" in str(j):
+            dtypedict.update({i: sqlalchemy.types.Float(precision=3, asdecimal=True)})
+        if "int" in str(j):
+            dtypedict.update({i: sqlalchemy.types.INT()})
+
+    info(dtypedict)
+    return dtypedict
```

### Comparing `etl_csm_pet-0.0.3/Etl/Loader.py` & `etl_csm_pet-0.0.4/Etl/Loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import psycopg2
 from re import findall
 from logging import info, warning
 from sqlalchemy import create_engine
 from typing import Type
 from os import environ
-from .Helper import psql_insert_copy,timing
+from .Helper import psql_insert_copy,timing,sqlcol
 
 @timing
 def load_cloud(df:Type,bot:str) -> None:
     """
     Ira fazer o processo de carregamento para o RDS depois de processado.
+    Ira estipular os datatype para sqlalchemy
+    Em seu excption acrescentar nova coluna de acordo com o datatype que ela precisa
+    ARGS
+    df = pd.DataFrame
     """
     engine_alchemy = create_engine(f"postgresql://tracking:{environ['SQL_PET_PASSWORD']}@pet-avi-chatbot-tracking-db.clarobrasil.mobi:5432/clean_data")
+    sql_dic = sqlcol(df) 
     tries = 10
     for _ in range(tries):
         try:
-            df.to_sql(f'{bot}_tracking_treated',engine_alchemy,if_exists = 'append',method = psql_insert_copy,index = False,chunksize = 10000)
+            df.to_sql(f'{bot}_tracking_treated',engine_alchemy,if_exists = 'append',method = psql_insert_copy,dtype = sql_dic ,index = False,chunksize = 10000)
             break
         except (Exception,psycopg2.Error) as error:
             warning("Fazendo novo conexao com a clean data para adicionar coluna!")
             engine = psycopg2.connect(
                 database = 'clean_data',
                 user = 'tracking',
                 password = environ['SQL_PET_PASSWORD'],
```

### Comparing `etl_csm_pet-0.0.3/Etl/Treatment_extras.py` & `etl_csm_pet-0.0.4/Etl/Treatment_extras.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.3/Etl/Treatment_tracking.py` & `etl_csm_pet-0.0.4/Etl/Treatment_tracking.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.3/Etl/Treatment_tracking_pme.py` & `etl_csm_pet-0.0.4/Etl/Treatment_tracking_pme.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.3/Etl/__init__.py` & `etl_csm_pet-0.0.4/Etl/__init__.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.3/LICENSE` & `etl_csm_pet-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.3/PKG-INFO` & `etl_csm_pet-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl_csm_pet
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm_pet-0.0.3/README.md` & `etl_csm_pet-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.3/etl_csm_pet.egg-info/PKG-INFO` & `etl_csm_pet-0.0.4/etl_csm_pet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-csm-pet
-Version: 0.0.3
+Version: 0.0.4
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm_pet-0.0.3/setup.py` & `etl_csm_pet-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Pacote de ETL'
 
 # Setting up
 setup(
     name = "etl_csm_pet",
     version = VERSION,
     author = "ingloriamori",
```


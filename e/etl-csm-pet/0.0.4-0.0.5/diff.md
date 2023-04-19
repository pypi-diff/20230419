# Comparing `tmp/etl_csm_pet-0.0.4.tar.gz` & `tmp/etl_csm_pet-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_csm_pet-0.0.4.tar", last modified: Wed Apr 19 17:44:04 2023, max compression
+gzip compressed data, was "etl_csm_pet-0.0.5.tar", last modified: Wed Apr 19 20:29:34 2023, max compression
```

## Comparing `etl_csm_pet-0.0.4.tar` & `etl_csm_pet-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 17:44:04.165247 etl_csm_pet-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-04-19 17:44:04.160245 etl_csm_pet-0.0.4/Etl/
--rw-rw-rw-   0        0        0     3381 2023-04-19 17:00:12.000000 etl_csm_pet-0.0.4/Etl/Execute.py
--rw-rw-rw-   0        0        0     1577 2023-04-19 17:00:12.000000 etl_csm_pet-0.0.4/Etl/Extrator.py
--rw-rw-rw-   0        0        0     2794 2023-04-19 17:33:43.000000 etl_csm_pet-0.0.4/Etl/Helper.py
--rw-rw-rw-   0        0        0     1978 2023-04-19 17:19:57.000000 etl_csm_pet-0.0.4/Etl/Loader.py
--rw-rw-rw-   0        0        0     4814 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.4/Etl/Treatment_extras.py
--rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm_pet-0.0.4/Etl/Treatment_tracking.py
--rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.4/Etl/Treatment_tracking_pme.py
--rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.4/Etl/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm_pet-0.0.4/LICENSE
--rw-rw-rw-   0        0        0      552 2023-04-19 17:44:04.164245 etl_csm_pet-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm_pet-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 17:44:04.164245 etl_csm_pet-0.0.4/etl_csm_pet.egg-info/
--rw-rw-rw-   0        0        0      552 2023-04-19 17:44:03.000000 etl_csm_pet-0.0.4/etl_csm_pet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-04-19 17:44:03.000000 etl_csm_pet-0.0.4/etl_csm_pet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 17:44:03.000000 etl_csm_pet-0.0.4/etl_csm_pet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-19 17:44:03.000000 etl_csm_pet-0.0.4/etl_csm_pet.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-19 17:44:03.000000 etl_csm_pet-0.0.4/etl_csm_pet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 17:44:04.165247 etl_csm_pet-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      937 2023-04-19 17:43:23.000000 etl_csm_pet-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:29:34.975407 etl_csm_pet-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-04-19 20:29:34.971408 etl_csm_pet-0.0.5/Etl/
+-rw-rw-rw-   0        0        0     3381 2023-04-19 20:28:52.000000 etl_csm_pet-0.0.5/Etl/Execute.py
+-rw-rw-rw-   0        0        0     1577 2023-04-19 20:28:52.000000 etl_csm_pet-0.0.5/Etl/Extrator.py
+-rw-rw-rw-   0        0        0     2812 2023-04-19 20:28:52.000000 etl_csm_pet-0.0.5/Etl/Helper.py
+-rw-rw-rw-   0        0        0     2023 2023-04-19 20:28:52.000000 etl_csm_pet-0.0.5/Etl/Loader.py
+-rw-rw-rw-   0        0        0     4918 2023-04-19 20:28:52.000000 etl_csm_pet-0.0.5/Etl/Treatment_extras.py
+-rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm_pet-0.0.5/Etl/Treatment_tracking.py
+-rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.5/Etl/Treatment_tracking_pme.py
+-rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm_pet-0.0.5/Etl/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm_pet-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0      552 2023-04-19 20:29:34.975407 etl_csm_pet-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm_pet-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 20:29:34.974407 etl_csm_pet-0.0.5/etl_csm_pet.egg-info/
+-rw-rw-rw-   0        0        0      552 2023-04-19 20:29:34.000000 etl_csm_pet-0.0.5/etl_csm_pet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      355 2023-04-19 20:29:34.000000 etl_csm_pet-0.0.5/etl_csm_pet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 20:29:34.000000 etl_csm_pet-0.0.5/etl_csm_pet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-19 20:29:34.000000 etl_csm_pet-0.0.5/etl_csm_pet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-19 20:29:34.000000 etl_csm_pet-0.0.5/etl_csm_pet.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 20:29:34.976407 etl_csm_pet-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      937 2023-04-19 20:29:04.000000 etl_csm_pet-0.0.5/setup.py
```

### Comparing `etl_csm_pet-0.0.4/Etl/Execute.py` & `etl_csm_pet-0.0.5/Etl/Execute.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.4/Etl/Extrator.py` & `etl_csm_pet-0.0.5/Etl/Extrator.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.4/Etl/Helper.py` & `etl_csm_pet-0.0.5/Etl/Helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         columns = ', '.join(['"{}"'.format(k) for k in keys])
         if table.schema:
             table_name = '{}.{}'.format(table.schema, table.name)
         else:
             table_name = table.name
         sql = 'COPY {} ({}) FROM STDIN WITH CSV'.format(
             table_name, columns)
+        info(sql)
         cur.copy_expert(sql=sql, file=s_buf)
 
 def map_substring(s, dict_map) -> dict:
     """
     Funcao helper mapeia as sub strings com facilidade
     ARGS
     s = pd.Series a ser interada por
@@ -70,17 +71,16 @@
     ARGS
     df, para acessar os objetos de colunas e datatypes
     """
     info("Formulando dict_map de datatype SQLalchemy")
     dtypedict = {}
     for i,j in zip(df.columns, df.dtypes):
         if "object" in str(j):
-            dtypedict.update({i: sqlalchemy.types.VARCHAR(length=300)})                 
+            dtypedict.update({i: sqlalchemy.types.VARCHAR(length=2000)})                 
         if "datetime" in str(j):
             dtypedict.update({i: sqlalchemy.types.DateTime()})
         if "float" in str(j):
             dtypedict.update({i: sqlalchemy.types.Float(precision=3, asdecimal=True)})
         if "int" in str(j):
             dtypedict.update({i: sqlalchemy.types.INT()})
-
     info(dtypedict)
     return dtypedict
```

### Comparing `etl_csm_pet-0.0.4/Etl/Loader.py` & `etl_csm_pet-0.0.5/Etl/Loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import psycopg2
+import json
 from re import findall
 from logging import info, warning
 from sqlalchemy import create_engine
 from typing import Type
 from os import environ
 from .Helper import psql_insert_copy,timing,sqlcol
 
@@ -13,26 +14,27 @@
     Ira estipular os datatype para sqlalchemy
     Em seu excption acrescentar nova coluna de acordo com o datatype que ela precisa
     ARGS
     df = pd.DataFrame
     """
     engine_alchemy = create_engine(f"postgresql://tracking:{environ['SQL_PET_PASSWORD']}@pet-avi-chatbot-tracking-db.clarobrasil.mobi:5432/clean_data")
     sql_dic = sqlcol(df) 
-    tries = 10
+    tries = 5
+
     for _ in range(tries):
         try:
-            df.to_sql(f'{bot}_tracking_treated',engine_alchemy,if_exists = 'append',method = psql_insert_copy,dtype = sql_dic ,index = False,chunksize = 10000)
-            break
-        except (Exception,psycopg2.Error) as error:
-            warning("Fazendo novo conexao com a clean data para adicionar coluna!")
+            df.to_sql(f'{bot}_tracking_treated',engine_alchemy,dtype = sql_dic ,method = psql_insert_copy,if_exists='append',index = False,chunksize = 10000)
+        except  (Exception,psycopg2.Error) as error:
+            warning("Tivemos um erro", error)
+            warning("Vou executar um handler para ver se consigo resolver!")         
             engine = psycopg2.connect(
                 database = 'clean_data',
                 user = 'tracking',
-                password = environ['SQL_PET_PASSWORD'],
-                host = 'pet-avi-chatbot-tracking-db.clarobrasil.mobi',
+                password = environ['SQL_PRD_PASSWORD'],
+                host = 'prd-avi-chatbot-tracking-db.clarobrasil.mobi',
                 port = '5432',
             )
             cursor = engine.cursor()
             column = findall('"(.*?)"',str(error))[0]
             warning(f"Tive que acrescentar mais uma coluna ao seu dataframe ja existente a coluna foi {column}")
             query = f"""
             ALTER TABLE {bot}_tracking_treated
@@ -40,8 +42,8 @@
             """
             info(query)
             cursor.execute(query)
             engine.commit()
             # Sempre fazer esse commit pelo amor
             tries -= 1
         if tries == 0:
-            warning("E não deu eu puis maximo de colunas que podia")
+            warning("E não deu eu puis maximo de colunas que podia")
```

### Comparing `etl_csm_pet-0.0.4/Etl/Treatment_extras.py` & `etl_csm_pet-0.0.5/Etl/Treatment_extras.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,15 +92,18 @@
                 'alternative_installation_period_day':str,
                 'type_of_instalation':str,
                 'redemption_laststate':str,
                 'ticket_id':str,
                 'userphone_plus':str,
                 'incentive_redirection':str,
                 'api_customercontracts_error':str,
-                'api_homepassed_error':str
+                'api_homepassed_error':str,
+                'plan_value':str,
+                'plan_offer':str,
+                'plan_name':str
                 }
     dtypes = {}
     # Mapa dos dtypes do dataframe atual
     for k in list(extras_df.columns):
         try:
             dtypes[k] = general_map[k]
         except KeyError as error:
```

### Comparing `etl_csm_pet-0.0.4/Etl/Treatment_tracking.py` & `etl_csm_pet-0.0.5/Etl/Treatment_tracking.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.4/Etl/Treatment_tracking_pme.py` & `etl_csm_pet-0.0.5/Etl/Treatment_tracking_pme.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.4/Etl/__init__.py` & `etl_csm_pet-0.0.5/Etl/__init__.py`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.4/LICENSE` & `etl_csm_pet-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.4/PKG-INFO` & `etl_csm_pet-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl_csm_pet
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm_pet-0.0.4/README.md` & `etl_csm_pet-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `etl_csm_pet-0.0.4/etl_csm_pet.egg-info/PKG-INFO` & `etl_csm_pet-0.0.5/etl_csm_pet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-csm-pet
-Version: 0.0.4
+Version: 0.0.5
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm_pet-0.0.4/setup.py` & `etl_csm_pet-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Pacote de ETL'
 
 # Setting up
 setup(
     name = "etl_csm_pet",
     version = VERSION,
     author = "ingloriamori",
```


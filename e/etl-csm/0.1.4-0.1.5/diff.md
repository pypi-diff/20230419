# Comparing `tmp/etl_csm-0.1.4.tar.gz` & `tmp/etl_csm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etl_csm-0.1.4.tar", last modified: Mon Apr 17 14:48:33 2023, max compression
+gzip compressed data, was "etl_csm-0.1.5.tar", last modified: Wed Apr 19 20:20:28 2023, max compression
```

## Comparing `etl_csm-0.1.4.tar` & `etl_csm-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 14:48:33.068051 etl_csm-0.1.4/
-drwxrwxrwx   0        0        0        0 2023-04-17 14:48:33.063049 etl_csm-0.1.4/Etl/
--rw-rw-rw-   0        0        0     3379 2023-04-17 14:37:44.000000 etl_csm-0.1.4/Etl/Execute.py
--rw-rw-rw-   0        0        0     1547 2023-04-17 14:38:05.000000 etl_csm-0.1.4/Etl/Extrator.py
--rw-rw-rw-   0        0        0     1965 2023-04-12 17:53:53.000000 etl_csm-0.1.4/Etl/Helper.py
--rw-rw-rw-   0        0        0     1761 2023-04-17 14:38:26.000000 etl_csm-0.1.4/Etl/Loader.py
--rw-rw-rw-   0        0        0     4814 2023-04-12 17:53:53.000000 etl_csm-0.1.4/Etl/Treatment_extras.py
--rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm-0.1.4/Etl/Treatment_tracking.py
--rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm-0.1.4/Etl/Treatment_tracking_pme.py
--rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm-0.1.4/Etl/__init__.py
--rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm-0.1.4/LICENSE
--rw-rw-rw-   0        0        0      526 2023-04-17 14:48:33.067052 etl_csm-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 14:48:33.066049 etl_csm-0.1.4/etl_csm.egg-info/
--rw-rw-rw-   0        0        0      526 2023-04-17 14:48:32.000000 etl_csm-0.1.4/etl_csm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-04-17 14:48:32.000000 etl_csm-0.1.4/etl_csm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 14:48:32.000000 etl_csm-0.1.4/etl_csm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-04-17 14:48:32.000000 etl_csm-0.1.4/etl_csm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-17 14:48:32.000000 etl_csm-0.1.4/etl_csm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 14:48:33.068051 etl_csm-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      911 2023-04-17 14:48:31.000000 etl_csm-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 20:20:28.808410 etl_csm-0.1.5/
+drwxrwxrwx   0        0        0        0 2023-04-19 20:20:28.803407 etl_csm-0.1.5/Etl/
+-rw-rw-rw-   0        0        0     3379 2023-04-19 19:01:38.000000 etl_csm-0.1.5/Etl/Execute.py
+-rw-rw-rw-   0        0        0     1547 2023-04-19 19:01:38.000000 etl_csm-0.1.5/Etl/Extrator.py
+-rw-rw-rw-   0        0        0     2779 2023-04-19 19:48:06.000000 etl_csm-0.1.5/Etl/Helper.py
+-rw-rw-rw-   0        0        0     2010 2023-04-19 19:51:35.000000 etl_csm-0.1.5/Etl/Loader.py
+-rw-rw-rw-   0        0        0     4814 2023-04-19 19:01:38.000000 etl_csm-0.1.5/Etl/Treatment_extras.py
+-rw-rw-rw-   0        0        0    12405 2023-04-13 16:55:54.000000 etl_csm-0.1.5/Etl/Treatment_tracking.py
+-rw-rw-rw-   0        0        0      656 2023-04-12 17:53:53.000000 etl_csm-0.1.5/Etl/Treatment_tracking_pme.py
+-rw-rw-rw-   0        0        0      616 2023-04-12 17:53:53.000000 etl_csm-0.1.5/Etl/__init__.py
+-rw-rw-rw-   0        0        0     1091 2023-03-14 18:25:25.000000 etl_csm-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0      526 2023-04-19 20:20:28.807407 etl_csm-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2023-04-14 13:30:45.000000 etl_csm-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 20:20:28.807407 etl_csm-0.1.5/etl_csm.egg-info/
+-rw-rw-rw-   0        0        0      526 2023-04-19 20:20:28.000000 etl_csm-0.1.5/etl_csm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2023-04-19 20:20:28.000000 etl_csm-0.1.5/etl_csm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 20:20:28.000000 etl_csm-0.1.5/etl_csm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-04-19 20:20:28.000000 etl_csm-0.1.5/etl_csm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-04-19 20:20:28.000000 etl_csm-0.1.5/etl_csm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 20:20:28.808410 etl_csm-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      911 2023-04-19 20:20:25.000000 etl_csm-0.1.5/setup.py
```

### Comparing `etl_csm-0.1.4/Etl/Execute.py` & `etl_csm-0.1.5/Etl/Execute.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.4/Etl/Extrator.py` & `etl_csm-0.1.5/Etl/Extrator.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.4/Etl/Helper.py` & `etl_csm-0.1.5/Etl/Helper.py`

 * *Files 12% similar despite different names*

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
@@ -56,8 +57,29 @@
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
+    Funcao que mapeia os datatype das tabelas e retorna o datatype adequado do SQLalchemy
+    ARGS
+    df, para acessar os objetos de colunas e datatypes
+    """
+    info("Formulando dict_map de datatype SQLalchemy")
+    dtypedict = {}
+    for i,j in zip(df.columns, df.dtypes):
+        if "object" in str(j):
+            dtypedict.update({i: sqlalchemy.types.VARCHAR(length=3000)})                 
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

### Comparing `etl_csm-0.1.4/Etl/Loader.py` & `etl_csm-0.1.5/Etl/Loader.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,34 @@
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
     engine_alchemy = create_engine(f"postgresql://tracking:{environ['SQL_PRD_PASSWORD']}@prd-avi-chatbot-tracking-db.clarobrasil.mobi:5432/clean_data")
-    tries = 10
+    sql_dic = sqlcol(df) 
+    tries = 5
+
     for _ in range(tries):
         try:
-            df.to_sql(f'{bot}_tracking_treated',engine_alchemy,if_exists = 'append',method = psql_insert_copy,index = False,chunksize = 10000)
-            break
-        except (Exception,psycopg2.Error) as error:
-            warning("Fazendo novo conexao com a clean data para adicionar coluna!")
+            df.to_sql(f'{bot}_tracking_treated',engine_alchemy,dtype = sql_dic ,method = psql_insert_copy,if_exists = 'append',index = False,chunksize = 10000)
+        except  (Exception,psycopg2.Error) as error:
+            warning("Tivemos um erro", error)
+            warning("Vou executar um handler para ver se consigo resolver!")         
             engine = psycopg2.connect(
                 database = 'clean_data',
                 user = 'tracking',
                 password = environ['SQL_PRD_PASSWORD'],
                 host = 'prd-avi-chatbot-tracking-db.clarobrasil.mobi',
                 port = '5432',
             )
```

### Comparing `etl_csm-0.1.4/Etl/Treatment_extras.py` & `etl_csm-0.1.5/Etl/Treatment_extras.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.4/Etl/Treatment_tracking.py` & `etl_csm-0.1.5/Etl/Treatment_tracking.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.4/Etl/Treatment_tracking_pme.py` & `etl_csm-0.1.5/Etl/Treatment_tracking_pme.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.4/Etl/__init__.py` & `etl_csm-0.1.5/Etl/__init__.py`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.4/LICENSE` & `etl_csm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.4/PKG-INFO` & `etl_csm-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl_csm
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.1.4/README.md` & `etl_csm-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `etl_csm-0.1.4/etl_csm.egg-info/PKG-INFO` & `etl_csm-0.1.5/etl_csm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etl-csm
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pacote de ETL
 Home-page: https://gitdev.clarobrasil.mobi/vendas-claro/csm/etl
 Author: ingloriamori
 Author-email: francisco.froes@globalhitss.com.br
 License: MIT
 Keywords: python,etl
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `etl_csm-0.1.4/setup.py` & `etl_csm-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.1.4'
+VERSION = '0.1.5'
 DESCRIPTION = 'Pacote de ETL'
 
 # Setting up
 setup(
     name = "etl_csm",
     version = VERSION,
     author = "ingloriamori",
```


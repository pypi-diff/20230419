# Comparing `tmp/smart-scrap-0.1.1.tar.gz` & `tmp/smart-scrap-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart-scrap-0.1.1.tar", last modified: Mon Apr 17 11:17:58 2023, max compression
+gzip compressed data, was "smart-scrap-0.1.2.tar", last modified: Wed Apr 19 05:46:32 2023, max compression
```

## Comparing `smart-scrap-0.1.1.tar` & `smart-scrap-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-04-17 11:17:58.358426 smart-scrap-0.1.1/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      398 2023-04-17 11:17:58.358261 smart-scrap-0.1.1/PKG-INFO
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-04-17 11:17:58.356569 smart-scrap-0.1.1/db/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)        0 2023-04-17 09:28:05.000000 smart-scrap-0.1.1/db/__init__.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)     3479 2023-04-17 09:47:28.000000 smart-scrap-0.1.1/db/main.py
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       38 2023-04-17 11:17:58.358475 smart-scrap-0.1.1/setup.cfg
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      664 2023-04-17 11:17:35.000000 smart-scrap-0.1.1/setup.py
-drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-04-17 11:17:58.358040 smart-scrap-0.1.1/smart_scrap.egg-info/
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      398 2023-04-17 11:17:58.000000 smart-scrap-0.1.1/smart_scrap.egg-info/PKG-INFO
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)      212 2023-04-17 11:17:58.000000 smart-scrap-0.1.1/smart_scrap.egg-info/SOURCES.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)        1 2023-04-17 11:17:58.000000 smart-scrap-0.1.1/smart_scrap.egg-info/dependency_links.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)       36 2023-04-17 11:17:58.000000 smart-scrap-0.1.1/smart_scrap.egg-info/entry_points.txt
--rw-r--r--   0 nikhilsaraf   (501) staff       (20)        3 2023-04-17 11:17:58.000000 smart-scrap-0.1.1/smart_scrap.egg-info/top_level.txt
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-04-19 05:46:32.937033 smart-scrap-0.1.2/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      398 2023-04-19 05:46:32.936864 smart-scrap-0.1.2/PKG-INFO
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-04-19 05:46:32.935759 smart-scrap-0.1.2/db/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       66 2023-04-19 03:36:36.000000 smart-scrap-0.1.2/db/__init__.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     2399 2023-04-19 03:44:35.000000 smart-scrap-0.1.2/db/cache.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      622 2023-04-18 06:36:33.000000 smart-scrap-0.1.2/db/connection.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     3173 2023-04-19 05:44:48.000000 smart-scrap-0.1.2/db/main.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)     5347 2023-04-19 03:32:39.000000 smart-scrap-0.1.2/db/map.py
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       38 2023-04-19 05:46:32.937081 smart-scrap-0.1.2/setup.cfg
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      664 2023-04-19 05:46:20.000000 smart-scrap-0.1.2/setup.py
+drwxr-xr-x   0 nikhilsaraf   (501) staff       (20)        0 2023-04-19 05:46:32.936606 smart-scrap-0.1.2/smart_scrap.egg-info/
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      398 2023-04-19 05:46:32.000000 smart-scrap-0.1.2/smart_scrap.egg-info/PKG-INFO
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)      251 2023-04-19 05:46:32.000000 smart-scrap-0.1.2/smart_scrap.egg-info/SOURCES.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)        1 2023-04-19 05:46:32.000000 smart-scrap-0.1.2/smart_scrap.egg-info/dependency_links.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)       36 2023-04-19 05:46:32.000000 smart-scrap-0.1.2/smart_scrap.egg-info/entry_points.txt
+-rw-r--r--   0 nikhilsaraf   (501) staff       (20)        3 2023-04-19 05:46:32.000000 smart-scrap-0.1.2/smart_scrap.egg-info/top_level.txt
```

### Comparing `smart-scrap-0.1.1/db/main.py` & `smart-scrap-0.1.2/db/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,31 @@
 import os
 import subprocess
 import sys
 import argparse
 import os.path
+import pandas as pd
 
+from .connection import query
 
-def download(args):
-    import psycopg2
 
-    pg_user = os.environ['PG_USER']
-    pg_password = os.environ['PG_PASSWORD']
-    pg_host = os.environ['PG_HOST']
-    pg_dbname = os.environ['PG_DBNAME']
-    # Set up database connection
-    conn = psycopg2.connect(dbname=pg_dbname, user=pg_user,
-                            password=pg_password, host=pg_host, port='5432')
-    cur = conn.cursor()
-
-    # Execute query and fetch results
-    cur.execute(args.query)
-    results = cur.fetchall()
-
-    # Write results to output file
-    with open(args.output_file, 'w') as f:
-        # Write header row with column names
-        col_names = [desc[0] for desc in cur.description]
-        f.write(','.join(col_names) + '\n')
-
-        # Write data rows
-        for row in results:
-            f.write(','.join(str(val) for val in row) + '\n')
-
-    # Close database connection
-    cur.close()
-    conn.close()
+def download(args):
+    cols, results = query(args.query)
+    print('downloading')
+    pd.DataFrame(results, columns=[desc[0] for desc in cols]).to_csv(
+        args.output_file, index=False)
+    # # Write results to output file
+    # with open(args.output_file, 'w') as f:
+    #     # Write header row with column names
+    #     col_names = [desc[0] for desc in cols]
+    #     f.write(','.join(col_names) + '\n')
+
+    #     # Write data rows
+    #     for row in results:
+    #         f.write(','.join(str(val) for val in row) + '\n')
 
 
 def upload(args):
     # Read environment variables
     pg_user = os.environ['PG_USER']
     pg_password = os.environ['PG_PASSWORD']
     pg_host = os.environ['PG_HOST']
```

### Comparing `smart-scrap-0.1.1/setup.py` & `smart-scrap-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="smart-scrap",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "db = db.main:main",
         ],
     },
     install_requires=[
```


# Comparing `tmp/rdjohns_pg-1.5.5.tar.gz` & `tmp/rdjohns_pg-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdjohns_pg-1.5.5.tar", last modified: Fri Mar 24 12:55:29 2023, max compression
+gzip compressed data, was "rdjohns_pg-1.6.0.tar", last modified: Wed Apr 19 09:16:14 2023, max compression
```

## Comparing `rdjohns_pg-1.5.5.tar` & `rdjohns_pg-1.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 12:55:29.968069 rdjohns_pg-1.5.5/
--rw-rw-rw-   0        0        0     1088 2022-09-06 08:48:21.000000 rdjohns_pg-1.5.5/LICENSE
--rw-rw-rw-   0        0        0      904 2023-03-24 12:55:29.967094 rdjohns_pg-1.5.5/PKG-INFO
--rw-rw-rw-   0        0        0      442 2022-09-06 09:59:58.000000 rdjohns_pg-1.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-03-24 12:55:29.929012 rdjohns_pg-1.5.5/rdjohns_pg/
--rw-rw-rw-   0        0        0     3386 2022-12-06 10:24:32.000000 rdjohns_pg-1.5.5/rdjohns_pg/Datatable_Data.py
--rw-rw-rw-   0        0        0     7827 2022-11-17 16:53:02.000000 rdjohns_pg-1.5.5/rdjohns_pg/Datatable_JS.py
--rw-rw-rw-   0        0        0     5682 2022-12-07 15:16:09.000000 rdjohns_pg-1.5.5/rdjohns_pg/InsertComand.py
--rw-rw-rw-   0        0        0      873 2023-01-24 12:35:37.000000 rdjohns_pg-1.5.5/rdjohns_pg/Str_verification.py
--rw-rw-rw-   0        0        0     1704 2022-09-12 08:15:37.000000 rdjohns_pg-1.5.5/rdjohns_pg/Write_log.py
--rw-rw-rw-   0        0        0      195 2022-12-07 09:14:14.000000 rdjohns_pg-1.5.5/rdjohns_pg/__init__.py
--rw-rw-rw-   0        0        0      355 2022-09-09 13:28:53.000000 rdjohns_pg-1.5.5/rdjohns_pg/date.py
--rw-rw-rw-   0        0        0     4589 2023-03-24 12:53:47.000000 rdjohns_pg-1.5.5/rdjohns_pg/rdjohns_pg.py
-drwxrwxrwx   0        0        0        0 2023-03-24 12:55:29.964170 rdjohns_pg-1.5.5/rdjohns_pg.egg-info/
--rw-rw-rw-   0        0        0      904 2023-03-24 12:55:29.000000 rdjohns_pg-1.5.5/rdjohns_pg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2023-03-24 12:55:29.000000 rdjohns_pg-1.5.5/rdjohns_pg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 12:55:29.000000 rdjohns_pg-1.5.5/rdjohns_pg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-03-24 12:55:29.000000 rdjohns_pg-1.5.5/rdjohns_pg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-24 12:55:29.969046 rdjohns_pg-1.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1090 2023-03-24 12:54:14.000000 rdjohns_pg-1.5.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 09:16:14.093283 rdjohns_pg-1.6.0/
+-rw-rw-rw-   0        0        0     1088 2022-09-06 08:48:21.000000 rdjohns_pg-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0      904 2023-04-19 09:16:14.090349 rdjohns_pg-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0      442 2022-09-06 09:59:58.000000 rdjohns_pg-1.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 09:16:14.071798 rdjohns_pg-1.6.0/rdjohns_pg/
+-rw-rw-rw-   0        0        0     3386 2022-12-06 10:24:32.000000 rdjohns_pg-1.6.0/rdjohns_pg/Datatable_Data.py
+-rw-rw-rw-   0        0        0     7827 2022-11-17 16:53:02.000000 rdjohns_pg-1.6.0/rdjohns_pg/Datatable_JS.py
+-rw-rw-rw-   0        0        0     6847 2023-04-19 09:01:00.000000 rdjohns_pg-1.6.0/rdjohns_pg/InsertComand.py
+-rw-rw-rw-   0        0        0      873 2023-01-24 12:35:37.000000 rdjohns_pg-1.6.0/rdjohns_pg/Str_verification.py
+-rw-rw-rw-   0        0        0     1704 2022-09-12 08:15:37.000000 rdjohns_pg-1.6.0/rdjohns_pg/Write_log.py
+-rw-rw-rw-   0        0        0      195 2022-12-07 09:14:14.000000 rdjohns_pg-1.6.0/rdjohns_pg/__init__.py
+-rw-rw-rw-   0        0        0      355 2022-09-09 13:28:53.000000 rdjohns_pg-1.6.0/rdjohns_pg/date.py
+-rw-rw-rw-   0        0        0     4589 2023-03-24 12:53:47.000000 rdjohns_pg-1.6.0/rdjohns_pg/rdjohns_pg.py
+drwxrwxrwx   0        0        0        0 2023-04-19 09:16:14.089372 rdjohns_pg-1.6.0/rdjohns_pg.egg-info/
+-rw-rw-rw-   0        0        0      904 2023-04-19 09:16:13.000000 rdjohns_pg-1.6.0/rdjohns_pg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2023-04-19 09:16:13.000000 rdjohns_pg-1.6.0/rdjohns_pg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 09:16:13.000000 rdjohns_pg-1.6.0/rdjohns_pg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-19 09:16:13.000000 rdjohns_pg-1.6.0/rdjohns_pg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 09:16:14.094254 rdjohns_pg-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1090 2023-04-19 09:01:10.000000 rdjohns_pg-1.6.0/setup.py
```

### Comparing `rdjohns_pg-1.5.5/LICENSE` & `rdjohns_pg-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rdjohns_pg-1.5.5/PKG-INFO` & `rdjohns_pg-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdjohns_pg
-Version: 1.5.5
+Version: 1.6.0
 Summary: Use for the multiple delete, update or insert and select!
 Home-page: https://github.com/RDJohns/rdjohns_pg
 Author: David Johns
 Author-email: rakotonindrianajohns@email.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rdjohns_pg-1.5.5/rdjohns_pg/Datatable_Data.py` & `rdjohns_pg-1.6.0/rdjohns_pg/Datatable_Data.py`

 * *Files identical despite different names*

### Comparing `rdjohns_pg-1.5.5/rdjohns_pg/Datatable_JS.py` & `rdjohns_pg-1.6.0/rdjohns_pg/Datatable_JS.py`

 * *Files identical despite different names*

### Comparing `rdjohns_pg-1.5.5/rdjohns_pg/InsertComand.py` & `rdjohns_pg-1.6.0/rdjohns_pg/InsertComand.py`

 * *Files 19% similar despite different names*

```diff
@@ -46,14 +46,46 @@
             retour = True#'success'
         else:
             retour = False#'error'
     else:
         retour = False#'Aucun'
     return retour
 ################################################################################################
+######  Insertion des données sur la table tableName dans la base de donnée connection #########
+################################################################################################
+def InsertReturnIDCommande(data,tableName,connection,id=False):
+    name = []
+    value = []
+    if len(data)>0:
+        sql =" INSERT INTO "+tableName+" ( "
+        for key in data:
+            if data[key]:
+                name.append(key)
+                value.append("'"+("''".join(str(data[key]).split("'")))+"'")
+        value = ','.join(value)
+        name = ','.join(name)
+        
+        sql +=name+") VALUES ("+value+")"
+        if id:
+            sql+=" RETURNING id"
+        sql+=";"
+        print(sql)
+        try:
+            cursor1= connections[connection].cursor()
+            cursor1.execute(sql)
+            result = cursor1.fetchall()
+            print(result)
+            cursor1.close()
+            if len(result)>0:
+                return result[0][0]
+        except:
+            return 0
+    else:
+        return 0
+################################################################################################
 #####  Mise à jour des données sur la table tableName dans la base de donnée connection ########
 ################################################################################################
 def UpdateCommande(data,tableName,base,where=' '):
     if len(data)>0:
         sql =" UPDATE "+tableName+" SET  "
         i = 0
         for key in data:
```

### Comparing `rdjohns_pg-1.5.5/rdjohns_pg/Str_verification.py` & `rdjohns_pg-1.6.0/rdjohns_pg/Str_verification.py`

 * *Files identical despite different names*

### Comparing `rdjohns_pg-1.5.5/rdjohns_pg/Write_log.py` & `rdjohns_pg-1.6.0/rdjohns_pg/Write_log.py`

 * *Files identical despite different names*

### Comparing `rdjohns_pg-1.5.5/rdjohns_pg/rdjohns_pg.py` & `rdjohns_pg-1.6.0/rdjohns_pg/rdjohns_pg.py`

 * *Files identical despite different names*

### Comparing `rdjohns_pg-1.5.5/rdjohns_pg.egg-info/PKG-INFO` & `rdjohns_pg-1.6.0/rdjohns_pg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rdjohns-pg
-Version: 1.5.5
+Version: 1.6.0
 Summary: Use for the multiple delete, update or insert and select!
 Home-page: https://github.com/RDJohns/rdjohns_pg
 Author: David Johns
 Author-email: rakotonindrianajohns@email.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `rdjohns_pg-1.5.5/setup.py` & `rdjohns_pg-1.6.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="rdjohns_pg",
-    version="1.5.5",
+    version="1.6.0",
     author="David Johns",
     author_email="rakotonindrianajohns@email.com",
     description="Use for the multiple delete, update or insert and select!",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/RDJohns/rdjohns_pg",
     packages=setuptools.find_packages(),
```


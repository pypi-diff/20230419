# Comparing `tmp/nriapp-1.1.11.tar.gz` & `tmp/nriapp-1.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nriapp-1.1.11.tar", last modified: Wed Apr 19 14:12:41 2023, max compression
+gzip compressed data, was "nriapp-1.1.12.tar", last modified: Wed Apr 19 15:02:09 2023, max compression
```

## Comparing `nriapp-1.1.11.tar` & `nriapp-1.1.12.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.133888 nriapp-1.1.11/
--rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.11/LICENSE
--rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.11/MANIFEST.in
--rw-rw-rw-   0        0        0      273 2023-04-19 14:12:41.133888 nriapp-1.1.11/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.11/README
--rw-rw-rw-   0        0        0      336 2023-04-19 14:12:28.000000 nriapp-1.1.11/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-04-19 14:12:41.133888 nriapp-1.1.11/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-04-19 14:12:29.000000 nriapp-1.1.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.102688 nriapp-1.1.11/src/
-drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.118288 nriapp-1.1.11/src/nriapp/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/__init__.py
--rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.11/src/nriapp/changelog.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.118288 nriapp-1.1.11/src/nriapp/config/
--rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/config/__init__.py
--rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/config/config.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.118288 nriapp-1.1.11/src/nriapp/core/
--rw-rw-rw-   0        0        0        0 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/core/__init__.py
--rw-rw-rw-   0        0        0     1520 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/core/abuseipdbapi.py
--rw-rw-rw-   0        0        0    13766 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/core/dataexplorer.py
--rw-rw-rw-   0        0        0    25825 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/core/msgraphapi.py
--rw-rw-rw-   0        0        0   101391 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/core/mssentinelapi.py
--rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/core/multifactor.py
--rw-rw-rw-   0        0        0      640 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/core/vtquery.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.133888 nriapp-1.1.11/src/nriapp/helper/
--rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/helper/__init__.py
--rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/helper/doc.py
--rw-rw-rw-   0        0        0      246 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/helper/excel.py
--rw-rw-rw-   0        0        0     8482 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/helper/login.py
--rw-rw-rw-   0        0        0     2443 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/helper/pylog.py
--rw-rw-rw-   0        0        0     1247 2023-03-02 07:59:35.000000 nriapp-1.1.11/src/nriapp/helper/requestheader.py
--rw-rw-rw-   0        0        0       92 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/helper/visualization.py
-drwxrwxrwx   0        0        0        0 2023-04-19 14:12:41.118288 nriapp-1.1.11/src/nriapp/nriapp.egg-info/
--rw-rw-rw-   0        0        0      273 2023-04-19 14:12:41.000000 nriapp-1.1.11/src/nriapp/nriapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1024 2023-04-19 14:12:41.000000 nriapp-1.1.11/src/nriapp/nriapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 14:12:41.000000 nriapp-1.1.11/src/nriapp/nriapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-04-19 14:12:41.000000 nriapp-1.1.11/src/nriapp/nriapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-04-19 14:12:41.000000 nriapp-1.1.11/src/nriapp/nriapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35379 2023-04-19 13:47:32.000000 nriapp-1.1.11/src/nriapp/nriapp.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.499948 nriapp-1.1.12/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.12/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.12/MANIFEST.in
+-rw-rw-rw-   0        0        0      273 2023-04-19 15:02:09.499948 nriapp-1.1.12/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.12/README
+-rw-rw-rw-   0        0        0      336 2023-04-19 14:16:22.000000 nriapp-1.1.12/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-04-19 15:02:09.499948 nriapp-1.1.12/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-04-19 15:01:23.000000 nriapp-1.1.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.484348 nriapp-1.1.12/src/
+drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.499948 nriapp-1.1.12/src/nriapp/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/__init__.py
+-rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.12/src/nriapp/changelog.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.499948 nriapp-1.1.12/src/nriapp/config/
+-rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/config/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/config/config.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.499948 nriapp-1.1.12/src/nriapp/core/
+-rw-rw-rw-   0        0        0        0 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/core/__init__.py
+-rw-rw-rw-   0        0        0     1520 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/core/abuseipdbapi.py
+-rw-rw-rw-   0        0        0    13961 2023-04-19 14:54:34.000000 nriapp-1.1.12/src/nriapp/core/dataexplorer.py
+-rw-rw-rw-   0        0        0    25938 2023-04-19 14:57:41.000000 nriapp-1.1.12/src/nriapp/core/msgraphapi.py
+-rw-rw-rw-   0        0        0   101391 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/core/mssentinelapi.py
+-rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/core/multifactor.py
+-rw-rw-rw-   0        0        0      640 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/core/vtquery.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.499948 nriapp-1.1.12/src/nriapp/helper/
+-rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/helper/__init__.py
+-rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/helper/doc.py
+-rw-rw-rw-   0        0        0      246 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/helper/excel.py
+-rw-rw-rw-   0        0        0     8482 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/helper/login.py
+-rw-rw-rw-   0        0        0     2443 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/helper/pylog.py
+-rw-rw-rw-   0        0        0     1247 2023-03-02 07:59:35.000000 nriapp-1.1.12/src/nriapp/helper/requestheader.py
+-rw-rw-rw-   0        0        0       92 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/helper/visualization.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:02:09.484348 nriapp-1.1.12/src/nriapp/nriapp.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-04-19 15:02:09.000000 nriapp-1.1.12/src/nriapp/nriapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1024 2023-04-19 15:02:09.000000 nriapp-1.1.12/src/nriapp/nriapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 15:02:09.000000 nriapp-1.1.12/src/nriapp/nriapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-04-19 15:02:09.000000 nriapp-1.1.12/src/nriapp/nriapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-04-19 15:02:09.000000 nriapp-1.1.12/src/nriapp/nriapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35379 2023-04-19 13:47:32.000000 nriapp-1.1.12/src/nriapp/nriapp.py
```

### Comparing `nriapp-1.1.11/LICENSE` & `nriapp-1.1.12/LICENSE`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.11/setup.py` & `nriapp-1.1.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #with open('requirements.txt') as f:
 #    requirements = f.read().splitlines()
 
 
 setup(
    name='nriapp',
-   version='1.1.11',
+   version='1.1.12',
    description='This is an internal tool for crawling MS 365 Defender web with NRI',
     license='MIT',
    author='Llallum Victoria',
    author_email='llallumvictoria@gmail.com',
 #   packages=find_packages('src'),
    package_dir = {'':'src/nriapp'},
```

### Comparing `nriapp-1.1.11/src/nriapp/changelog.txt` & `nriapp-1.1.12/src/nriapp/changelog.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.11/src/nriapp/core/abuseipdbapi.py` & `nriapp-1.1.12/src/nriapp/core/abuseipdbapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.11/src/nriapp/core/dataexplorer.py` & `nriapp-1.1.12/src/nriapp/core/dataexplorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 import pandas as pd
 import os
 import concurrent.futures
 from tqdm import tqdm
 import pickle, cloudpickle
 from datetime import date
 
+desktop = os.path.join(os.path.join(os.environ['USERPROFILE']), 'Desktop') 
+
 session_file = os.path.abspath(os.path.dirname(__file__)) + "\..\session\kusto.pkl"
 tenant_id = "bcf2d2a2-2dee-419b-971f-21e5170fbf84"
 KUSTO_URI = "https://kvcw1z66xgnuy00q1uhhzs.australiaeast.kusto.windows.net"
 KUSTO_INGEST_URI = "https://ingest-kvcw1z66xgnuy00q1uhhzs.australiaeast.kusto.windows.net"
 
 class DataIngestion():
     def __init__(self, kusto_uri=KUSTO_URI, kusto_ingest_uri=KUSTO_INGEST_URI, tenant_id=tenant_id):
@@ -90,21 +92,22 @@
     #    unique = sorted(list(set(ids).difference(to_ingest)))
         similar = sorted(list(set(event_ids).intersection(to_ingest)))
 
         for i in data[:]:
             if i["IncidentId"] in similar:
                 data.remove(i)
 
-        with open("incidents.tmp", "w") as file:
+        path = os.path.join(desktop, "incidents.tmp")
+        with open(path, "w") as file:
             for item in data:
                 file.write(json.dumps(item) + "\n")
         if data:
             ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="RawEventMapping")
-            self.client_ingest.ingest_from_file("incidents.tmp", ingestion_properties=ingestion_props)
-        os.remove("incidents.tmp")
+            self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
+        os.remove(path)
         return data
 
 
     def ingest_mfastats(self, data, database="Incidents", table="Multifactor"):
         item_list = '''
         Multifactor
         | extend items = parse_json(Items)
@@ -124,21 +127,22 @@
         .delete table AuditHistory records <|
         AuditHistory
         | extend item = parse_json(Items)
         | where toint(item.id) in (''' + pending + ''')
         '''
         response = self.client_query.execute(database, remove_list)
 
-        with open("audit.tmp", "w") as file:
+        path = os.path.join(desktop, "audit.tmp")
+        with open(path, "w") as file:
             for item in data:
                 file.write(json.dumps(item) + "\n")
         if data:
             ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="AuditHistoryMapping")
-            self.client_ingest.ingest_from_file("audit.tmp", ingestion_properties=ingestion_props)
-        os.remove("audit.tmp")
+            self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
+        os.remove(path)
         return data    
 
     def check_ingest_users_tag(self, database="Incidents", table="AzureAD"):
         tag = date.today().strftime("%Y-%m-%d")
 
         current_tags = '''
         AzureAD
@@ -167,22 +171,22 @@
         | project trim_start("ingest-by:", tostring(tag))
         '''
         response = self.client_query.execute(database, current_tags)        
         tags = [i[0] for i in response.primary_results[0].raw_rows]
         for i in tags:
             if tag == i:
                 return
-
-        with open("users.tmp", "w") as file:
+        path = os.path.join(desktop, "users.tmp")
+        with open(path, "w") as file:
             for item in data:
                 file.write(json.dumps(item) + "\n")
         if data:
             ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="FlatEventMapping", ingest_if_not_exists=[tag],ingest_by_tags=[tag], drop_by_tags=[tag])
-            self.client_ingest.ingest_from_file("users.tmp", ingestion_properties=ingestion_props)
-        os.remove("users.tmp")
+            self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
+        os.remove(path)
 
     def check_ingest_devices_tags(self, database="Incidents", table="IntuneDevices"):
         tag = date.today().strftime("%Y-%m-%d")
 
         current_tags = '''
         IntuneDevices
         | extend tags = tostring(extent_tags())
@@ -210,22 +214,22 @@
         | project trim_start("ingest-by:", tostring(tag))
         '''
         response = self.client_query.execute(database, current_tags)        
         tags = [i[0] for i in response.primary_results[0].raw_rows]
         for i in tags:
             if tag == i:
                 return
-
-        with open("devices.tmp", "w") as file:
+        path = os.path.join(desktop, "devices.tmp")
+        with open(path, "w") as file:
             for item in data:
                 file.write(json.dumps(item) + "\n")
         if data:
             ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="IntuneDevicesMapping", ingest_if_not_exists=[tag],ingest_by_tags=[tag], drop_by_tags=[tag])
-            self.client_ingest.ingest_from_file("devices.tmp", ingestion_properties=ingestion_props)
-        os.remove("devices.tmp")
+            self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
+        os.remove(path)
 
     def check_ingest_managed_devices_tag(self, database="Incidents", table="ManagedDevices"):
         tag = date.today().strftime("%Y-%m-%d")
 
         current_tags = '''
         ManagedDevices
         | extend tags = tostring(extent_tags())
@@ -254,21 +258,22 @@
         '''
         response = self.client_query.execute(database, current_tags)        
         tags = [i[0] for i in response.primary_results[0].raw_rows]
         for i in tags:
             if tag == i:
                 return
 
-        with open("managedDevices.tmp", "w") as file:
+        path = os.path.join(desktop, "managedDevices.tmp")
+        with open(path, "w") as file:
             for item in data:
                 file.write(json.dumps(item) + "\n")
         if data:
             ingestion_props = IngestionProperties(database=database,table=table,data_format=DataFormat.MULTIJSON, ingestion_mapping_reference="ManagedDevicesMapping", ingest_if_not_exists=[tag],ingest_by_tags=[tag], drop_by_tags=[tag]) 
-            self.client_ingest.ingest_from_file("managedDevices.tmp", ingestion_properties=ingestion_props)
-        os.remove("managedDevices.tmp")
+            self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
+        os.remove(path)
 
 
     def ingest_defender_agents(self, path, database="Incidents", table="DefenderAgents"):
         tag = date.today().strftime("%Y-%m-%d")
 
         ingestion_props =  IngestionProperties(database=database,table=table,data_format=DataFormat.CSV, ingestion_mapping_reference="DefenderAgents_mapping", additional_properties={'ignoreFirstRecord': 'true'},  ingest_if_not_exists=[tag],ingest_by_tags=[tag], drop_by_tags=[tag]) 
         result = self.client_ingest.ingest_from_file(path, ingestion_properties=ingestion_props)
```

### Comparing `nriapp-1.1.11/src/nriapp/core/msgraphapi.py` & `nriapp-1.1.12/src/nriapp/core/msgraphapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -643,13 +643,14 @@
         status = object["status"]
         while status != "completed":
             dbgPrint.debug(status)
             result = self.tryrequest(export_job_result, headers=headers)
             object = json.loads(result.text)
             status = object["status"]        
         
+        desktop = os.path.join(os.path.join(os.environ['USERPROFILE']), 'Desktop') 
         dbgPrint.debug(status)
         agents_file = self.tryrequest(object["url"])
         dbgPrint.debug(object["url"])
         z = zipfile.ZipFile(io.BytesIO(agents_file.content))
-        z.extract(id+".csv", path="")
-        return id + ".csv"
+        z.extract(id+".csv", path=desktop)
+        return os.path.join(desktop, id + ".csv")
```

### Comparing `nriapp-1.1.11/src/nriapp/core/mssentinelapi.py` & `nriapp-1.1.12/src/nriapp/core/mssentinelapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.11/src/nriapp/core/multifactor.py` & `nriapp-1.1.12/src/nriapp/core/multifactor.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.11/src/nriapp/core/vtquery.py` & `nriapp-1.1.12/src/nriapp/core/vtquery.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.11/src/nriapp/helper/doc.py` & `nriapp-1.1.12/src/nriapp/helper/doc.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.11/src/nriapp/helper/login.py` & `nriapp-1.1.12/src/nriapp/helper/login.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.11/src/nriapp/helper/pylog.py` & `nriapp-1.1.12/src/nriapp/helper/pylog.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.11/src/nriapp/helper/requestheader.py` & `nriapp-1.1.12/src/nriapp/helper/requestheader.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.11/src/nriapp/nriapp.egg-info/SOURCES.txt` & `nriapp-1.1.12/src/nriapp/nriapp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.11/src/nriapp/nriapp.py` & `nriapp-1.1.12/src/nriapp/nriapp.py`

 * *Files identical despite different names*


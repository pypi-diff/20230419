# Comparing `tmp/customdbcred-0.3.tar.gz` & `tmp/customdbcred-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customdbcred-0.3.tar", last modified: Mon Apr 17 13:37:14 2023, max compression
+gzip compressed data, was "customdbcred-0.4.tar", last modified: Wed Apr 19 10:25:50 2023, max compression
```

## Comparing `customdbcred-0.3.tar` & `customdbcred-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 13:37:14.588815 customdbcred-0.3/
--rw-rw-rw-   0        0        0       57 2023-04-17 13:37:14.587814 customdbcred-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 13:37:14.562380 customdbcred-0.3/customdbcred/
--rw-rw-rw-   0        0        0     1931 2023-04-17 10:25:52.000000 customdbcred-0.3/customdbcred/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:37:14.582814 customdbcred-0.3/customdbcred.egg-info/
--rw-rw-rw-   0        0        0       57 2023-04-17 13:37:14.000000 customdbcred-0.3/customdbcred.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-04-17 13:37:14.000000 customdbcred-0.3/customdbcred.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 13:37:14.000000 customdbcred-0.3/customdbcred.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-04-17 13:37:14.000000 customdbcred-0.3/customdbcred.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 13:37:14.584807 customdbcred-0.3/customstatuscodes/
--rw-rw-rw-   0        0        0     8080 2023-03-25 11:42:47.000000 customdbcred-0.3/customstatuscodes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:37:14.585822 customdbcred-0.3/customvalidator/
--rw-rw-rw-   0        0        0     1387 2023-04-17 13:34:13.000000 customdbcred-0.3/customvalidator/__init__.py
--rw-rw-rw-   0        0        0       42 2023-04-17 13:37:14.588815 customdbcred-0.3/setup.cfg
--rw-rw-rw-   0        0        0      201 2023-04-17 13:37:06.000000 customdbcred-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:25:50.951401 customdbcred-0.4/
+-rw-rw-rw-   0        0        0       57 2023-04-19 10:25:50.950404 customdbcred-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-19 10:25:50.922253 customdbcred-0.4/customdbcred/
+-rw-rw-rw-   0        0        0     2171 2023-04-19 10:23:36.000000 customdbcred-0.4/customdbcred/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:25:50.936811 customdbcred-0.4/customdbcred.egg-info/
+-rw-rw-rw-   0        0        0       57 2023-04-19 10:25:50.000000 customdbcred-0.4/customdbcred.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-04-19 10:25:50.000000 customdbcred-0.4/customdbcred.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 10:25:50.000000 customdbcred-0.4/customdbcred.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-04-19 10:25:50.000000 customdbcred-0.4/customdbcred.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 10:25:50.942852 customdbcred-0.4/customstatuscodes/
+-rw-rw-rw-   0        0        0     8080 2023-04-13 12:37:42.000000 customdbcred-0.4/customstatuscodes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-19 10:25:50.949404 customdbcred-0.4/customvalidator/
+-rw-rw-rw-   0        0        0     1404 2023-04-17 13:43:49.000000 customdbcred-0.4/customvalidator/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-04-19 10:25:50.951401 customdbcred-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      201 2023-04-19 10:25:05.000000 customdbcred-0.4/setup.py
```

### Comparing `customdbcred-0.3/customdbcred/__init__.py` & `customdbcred-0.4/customdbcred/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Custom Module to fetch database credentials
-import logging
 from functools import wraps
-
+import json
 from azure.keyvault.secrets import SecretClient
 from azure.identity import ClientSecretCredential
 
+import logging
+
 logger_error = logging.getLogger('error_logs')
 
 
 def get_db_cred(func):
     @wraps(func)
     def wrapper_func(req):
         try:
@@ -18,18 +19,21 @@
             keyVaultName = "myappkv"
             KVUri = f"https://{keyVaultName}.vault.azure.net"
             # credential = DefaultAzureCredential()
             credential = ClientSecretCredential(tenant_id='26afc1b1-8393-439d-aa1a-483105d77dc3',
                                                 client_id='9d2fe19f-47e6-498f-b384-6f94b0d55500',
                                                 client_secret='lwk8Q~4LbZTagzrC6l0bpwrmraDrEQIalVZnfaf1')
             client = SecretClient(vault_url=KVUri, credential=credential)
-            server = client.get_secret("SERVER").value
-            database = client.get_secret("DATABASE").value
-            username = client.get_secret("USERNAME").value
-            password = client.get_secret("PASSWORD").value
+            dbcred = client.get_secret("DATABASECRED").value
+            cred = json.loads(dbcred)
+            # server = client.get_secret("SERVER").value
+            # database = client.get_secret("DATABASE").value
+            # username = client.get_secret("USERNAME").value
+            # password = client.get_secret("PASSWORD").value
+            server,database,username,password = cred['SERVER'], cred['DATABASE'], cred['USERNAME'], cred['PASSWORD']
             driver = '{ODBC Driver 17 for SQL Server}'
             output_json = dict(zip(["server", "database", "username", "password", "driver"],
                                    [server, database, username, password, driver]))
             request_data = req.get_json()
             request_data.update(output_json)
             result = func(request_data)
             return result
```

### Comparing `customdbcred-0.3/customstatuscodes/__init__.py` & `customdbcred-0.4/customstatuscodes/__init__.py`

 * *Files identical despite different names*

### Comparing `customdbcred-0.3/customvalidator/__init__.py` & `customdbcred-0.4/customvalidator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         data = data.get_json()
         v = jsonschema.Draft4Validator(schema)
         logger.info(v)
         errors = sorted(v.iter_errors(data), key=lambda e: e.path)
         for error in errors:
             logger.info('json validation failed')
             flag = 452
-            output_json = dict(zip(['Status', 'Message'], [flag, error.message]))
+            output_json = dict(zip(['Status', 'Message', 'Payload'], [flag, error.message, None]))
             return output_json
         logger.info('schema validation done')
         output_json = dict(zip(['Status', 'Message', 'Payload'], [flag, 'schema validation done', None]))
         return output_json
     except Exception as ex:
         logger_error.error(f"Exception Encountered Exception is : {ex}", exc_info=1)
         output_json = dict(zip(['Status', 'Message', 'Payload'], [500, f"Exception encountered: {ex}", None]))
```


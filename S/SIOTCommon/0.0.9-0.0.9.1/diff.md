# Comparing `tmp/SIOTCommon-0.0.9.tar.gz` & `tmp/SIOTCommon-0.0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTCommon-0.0.9.tar", last modified: Mon Apr 17 13:14:13 2023, max compression
+gzip compressed data, was "SIOTCommon-0.0.9.1.tar", last modified: Wed Apr 19 16:50:21 2023, max compression
```

## Comparing `SIOTCommon-0.0.9.tar` & `SIOTCommon-0.0.9.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 13:14:13.739373 SIOTCommon-0.0.9/
--rw-rw-rw-   0        0        0      339 2023-04-17 13:14:13.738373 SIOTCommon-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.9/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-17 13:14:13.723371 SIOTCommon-0.0.9/SIOTC/
--rw-rw-rw-   0        0        0     1651 2023-04-17 13:12:10.000000 SIOTCommon-0.0.9/SIOTC/DatabaseLayer.py
--rw-rw-rw-   0        0        0     6805 2023-04-16 14:42:03.000000 SIOTCommon-0.0.9/SIOTC/Operations.py
--rw-rw-rw-   0        0        0      443 2023-04-12 16:56:02.000000 SIOTCommon-0.0.9/SIOTC/__init__.py
--rw-rw-rw-   0        0        0     1846 2023-04-12 16:52:19.000000 SIOTCommon-0.0.9/SIOTC/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-04-17 13:14:13.737372 SIOTCommon-0.0.9/SIOTCommon.egg-info/
--rw-rw-rw-   0        0        0      339 2023-04-17 13:14:13.000000 SIOTCommon-0.0.9/SIOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-17 13:14:13.000000 SIOTCommon-0.0.9/SIOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 13:14:13.000000 SIOTCommon-0.0.9/SIOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      636 2023-04-17 13:14:13.000000 SIOTCommon-0.0.9/SIOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-17 13:14:13.000000 SIOTCommon-0.0.9/SIOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 13:14:13.739373 SIOTCommon-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-04-17 13:12:17.000000 SIOTCommon-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:50:21.172391 SIOTCommon-0.0.9.1/
+-rw-rw-rw-   0        0        0      341 2023-04-19 16:50:21.171391 SIOTCommon-0.0.9.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.9.1/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 16:50:21.147395 SIOTCommon-0.0.9.1/SIOTC/
+-rw-rw-rw-   0        0        0     1851 2023-04-19 16:34:13.000000 SIOTCommon-0.0.9.1/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0     6846 2023-04-19 15:57:38.000000 SIOTCommon-0.0.9.1/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      443 2023-04-12 16:56:02.000000 SIOTCommon-0.0.9.1/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     2291 2023-04-19 16:48:43.000000 SIOTCommon-0.0.9.1/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-04-19 16:50:21.169390 SIOTCommon-0.0.9.1/SIOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      341 2023-04-19 16:50:20.000000 SIOTCommon-0.0.9.1/SIOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-19 16:50:20.000000 SIOTCommon-0.0.9.1/SIOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 16:50:20.000000 SIOTCommon-0.0.9.1/SIOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      636 2023-04-19 16:50:20.000000 SIOTCommon-0.0.9.1/SIOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 16:50:20.000000 SIOTCommon-0.0.9.1/SIOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 16:50:21.172391 SIOTCommon-0.0.9.1/setup.cfg
+-rw-rw-rw-   0        0        0      583 2023-04-19 16:33:39.000000 SIOTCommon-0.0.9.1/setup.py
```

### Comparing `SIOTCommon-0.0.9/SIOTC/DatabaseLayer.py` & `SIOTCommon-0.0.9.1/SIOTC/DatabaseLayer.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 from sqlalchemy.ext.automap import automap_base
 from sqlalchemy import create_engine, Table
 from sqlalchemy.orm import sessionmaker, scoped_session
+import os
+
+dir_path = '/home/ubuntu/config/'
+filename = 'db_config.txt'
+file_path = os.path.join(dir_path, filename)
+
+with open(file_path, 'w') as f:
+    # Write the connection string to the file
+    first_line = f.readline().strip()
 
 def GetSession():
     Base = automap_base()
-    engine = create_engine('postgresql://postgres:3485780@localhost:5432/sweiot', echo=True)
+    engine = create_engine(first_line, echo=True)
     Base.prepare(engine, reflect=True, schema='public')
     session_factory = sessionmaker(bind=engine)
     session = scoped_session(session_factory)
     return session, Base
 
 def GetModel(table_name):
     session, Base = GetSession()
```

### Comparing `SIOTCommon-0.0.9/SIOTC/Operations.py` & `SIOTCommon-0.0.9.1/SIOTC/Operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         # Check if value is provided
         assert value is not None, "Error: No value provided"
         # Get all rows from the specified table and column
         theTable = GetAllOfColumnFromTable(table, column)
         # Check if an error occurred during retrieval
         if(theTable == False):
             print('Error: No table exist with provided values')
-            return None, 404
+            return None, 'Error: No table exist with provided values'
         # If no error, query the row that matches the provided value
         else:
             return theTable.query.filter_by(value).first()
     return executeQuery(queryFunc, value, column, table)
 
 # Add to any table to the database. Currently checks if missing columns and database constraints
 def InsertToTable(table, values):
```

### Comparing `SIOTCommon-0.0.9/SIOTC/helperhttps.py` & `SIOTCommon-0.0.9.1/SIOTC/helperhttps.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from flask import request, jsonify
 from functools import wraps
 from flask_jwt_extended import get_current_user
 from enum import Enum
+import Operations
 import re
 
-class Role(Enum):
-    ADMIN = 0
-    USER = 1
+op = Operations
 
 # Checks what type of data is being sent and returns correct object
 def CheckContentType():
     content_type = request.headers.get('Content-Type')
     if content_type == 'application/json':
         print('Json Message received')
         return request.json
@@ -39,17 +38,28 @@
         print('Content not abled to be verified or it does not match the intended format')
         return False
     
 def VerifyMacContent(content):
     regex_pattern = '^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$'
     return bool(re.match(regex_pattern, content))
 
-def admin_required(func):
-    @wraps(func)
-    def wrapper(*args, **kwargs):
-        user = get_current_user()
+def admin_required(current_user):
+    @wraps(current_user)
+    def wrapper(current_user):
+        user = current_user.id
         roleId = user.role_id
 
-        if roleId != Role.ADMIN.value:
-            return jsonify({'message': 'You do not have permission to access this endpoint.'}), 401
-        return func(*args, **kwargs)
+        if roleId != op.GetTable('roles').query.filter_by(name='System Administrator').first():
+            return jsonify({'message': 'You do not have permission to access this endpoint.'}), 403
+        return current_user
+    return wrapper
+
+def ownership_required(current_user, table):
+    @wraps(current_user, table)
+    def wrapper(current_user, table):
+        user = current_user.id
+        deviceID = op.GetTable(table).query.filter_by(id=current_user.id).first()
+
+        if user != deviceID.user_id:
+            return jsonify({'message': 'User does not own device.'}), 403
+        return current_user
     return wrapper
```

### Comparing `SIOTCommon-0.0.9/SIOTCommon.egg-info/requires.txt` & `SIOTCommon-0.0.9.1/SIOTCommon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9/setup.py` & `SIOTCommon-0.0.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTCommon',
-    version='0.0.9',
+    version='0.0.9.1',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```


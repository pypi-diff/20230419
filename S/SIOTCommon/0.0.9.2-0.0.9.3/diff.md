# Comparing `tmp/SIOTCommon-0.0.9.2.tar.gz` & `tmp/SIOTCommon-0.0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTCommon-0.0.9.2.tar", last modified: Wed Apr 19 17:15:01 2023, max compression
+gzip compressed data, was "SIOTCommon-0.0.9.3.tar", last modified: Wed Apr 19 17:46:57 2023, max compression
```

## Comparing `SIOTCommon-0.0.9.2.tar` & `SIOTCommon-0.0.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 17:15:01.853420 SIOTCommon-0.0.9.2/
--rw-rw-rw-   0        0        0      341 2023-04-19 17:15:01.852419 SIOTCommon-0.0.9.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.9.2/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 17:15:01.825420 SIOTCommon-0.0.9.2/SIOTC/
--rw-rw-rw-   0        0        0     1851 2023-04-19 16:34:13.000000 SIOTCommon-0.0.9.2/SIOTC/DatabaseLayer.py
--rw-rw-rw-   0        0        0     6846 2023-04-19 15:57:38.000000 SIOTCommon-0.0.9.2/SIOTC/Operations.py
--rw-rw-rw-   0        0        0      443 2023-04-12 16:56:02.000000 SIOTCommon-0.0.9.2/SIOTC/__init__.py
--rw-rw-rw-   0        0        0     2284 2023-04-19 17:14:41.000000 SIOTCommon-0.0.9.2/SIOTC/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-04-19 17:15:01.850419 SIOTCommon-0.0.9.2/SIOTCommon.egg-info/
--rw-rw-rw-   0        0        0      341 2023-04-19 17:15:01.000000 SIOTCommon-0.0.9.2/SIOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-19 17:15:01.000000 SIOTCommon-0.0.9.2/SIOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 17:15:01.000000 SIOTCommon-0.0.9.2/SIOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      636 2023-04-19 17:15:01.000000 SIOTCommon-0.0.9.2/SIOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 17:15:01.000000 SIOTCommon-0.0.9.2/SIOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 17:15:01.854426 SIOTCommon-0.0.9.2/setup.cfg
--rw-rw-rw-   0        0        0      583 2023-04-19 17:14:56.000000 SIOTCommon-0.0.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:46:57.509160 SIOTCommon-0.0.9.3/
+-rw-rw-rw-   0        0        0      341 2023-04-19 17:46:57.508159 SIOTCommon-0.0.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.9.3/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 17:46:57.487158 SIOTCommon-0.0.9.3/SIOTC/
+-rw-rw-rw-   0        0        0     1851 2023-04-19 16:34:13.000000 SIOTCommon-0.0.9.3/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0     6846 2023-04-19 15:57:38.000000 SIOTCommon-0.0.9.3/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      443 2023-04-12 16:56:02.000000 SIOTCommon-0.0.9.3/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     2261 2023-04-19 17:46:24.000000 SIOTCommon-0.0.9.3/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:46:57.506159 SIOTCommon-0.0.9.3/SIOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      341 2023-04-19 17:46:57.000000 SIOTCommon-0.0.9.3/SIOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-19 17:46:57.000000 SIOTCommon-0.0.9.3/SIOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 17:46:57.000000 SIOTCommon-0.0.9.3/SIOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      636 2023-04-19 17:46:57.000000 SIOTCommon-0.0.9.3/SIOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 17:46:57.000000 SIOTCommon-0.0.9.3/SIOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 17:46:57.510158 SIOTCommon-0.0.9.3/setup.cfg
+-rw-rw-rw-   0        0        0      583 2023-04-19 17:46:54.000000 SIOTCommon-0.0.9.3/setup.py
```

### Comparing `SIOTCommon-0.0.9.2/SIOTC/DatabaseLayer.py` & `SIOTCommon-0.0.9.3/SIOTC/DatabaseLayer.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9.2/SIOTC/Operations.py` & `SIOTCommon-0.0.9.3/SIOTC/Operations.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9.2/SIOTC/helperhttps.py` & `SIOTCommon-0.0.9.3/SIOTC/helperhttps.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from flask import request, jsonify
+from flask import request, jsonify 
 from functools import wraps
-from flask_jwt_extended import get_current_user
+from flask_jwt_extended import get_jwt_identity
 from enum import Enum
 import SIOTC.Operations as op
 import re
 
 # Checks what type of data is being sent and returns correct object
 def CheckContentType():
     content_type = request.headers.get('Content-Type')
@@ -36,28 +36,29 @@
         print('Content not abled to be verified or it does not match the intended format')
         return False
     
 def VerifyMacContent(content):
     regex_pattern = '^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$'
     return bool(re.match(regex_pattern, content))
 
-def admin_required(current_user):
-    @wraps(current_user)
-    def wrapper(current_user):
-        user = current_user.id
+def admin_required(f):
+    @wraps(f)
+    def decorated_function(*args, **kwargs):
+        user = get_jwt_identity()
         roleId = user.role_id
 
         if roleId != op.GetTable('roles').query.filter_by(name='System Administrator').first():
             return jsonify({'message': 'You do not have permission to access this endpoint.'}), 403
-        return current_user
-    return wrapper
+        return f(*args, **kwargs)
 
-def ownership_required(current_user, table):
-    @wraps(current_user, table)
-    def wrapper(current_user, table):
-        user = current_user.id
-        deviceID = op.GetTable(table).query.filter_by(id=current_user.id).first()
+    return decorated_function
+
+def ownership_required(f):
+    @wraps(f)
+    def wrapper(*args, **kwargs):
+        user = get_jwt_identity()
+        deviceID = op.GetTable('devices').query.filter_by(id=user).first()
 
         if user != deviceID.user_id:
             return jsonify({'message': 'User does not own device.'}), 403
-        return current_user
+        return f(*args, **kwargs)
     return wrapper
```

### Comparing `SIOTCommon-0.0.9.2/SIOTCommon.egg-info/requires.txt` & `SIOTCommon-0.0.9.3/SIOTCommon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9.2/setup.py` & `SIOTCommon-0.0.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTCommon',
-    version='0.0.9.2',
+    version='0.0.9.3',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```


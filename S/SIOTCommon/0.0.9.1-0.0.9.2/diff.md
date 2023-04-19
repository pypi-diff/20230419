# Comparing `tmp/SIOTCommon-0.0.9.1.tar.gz` & `tmp/SIOTCommon-0.0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SIOTCommon-0.0.9.1.tar", last modified: Wed Apr 19 16:50:21 2023, max compression
+gzip compressed data, was "SIOTCommon-0.0.9.2.tar", last modified: Wed Apr 19 17:15:01 2023, max compression
```

## Comparing `SIOTCommon-0.0.9.1.tar` & `SIOTCommon-0.0.9.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 16:50:21.172391 SIOTCommon-0.0.9.1/
--rw-rw-rw-   0        0        0      341 2023-04-19 16:50:21.171391 SIOTCommon-0.0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.9.1/README.txt
-drwxrwxrwx   0        0        0        0 2023-04-19 16:50:21.147395 SIOTCommon-0.0.9.1/SIOTC/
--rw-rw-rw-   0        0        0     1851 2023-04-19 16:34:13.000000 SIOTCommon-0.0.9.1/SIOTC/DatabaseLayer.py
--rw-rw-rw-   0        0        0     6846 2023-04-19 15:57:38.000000 SIOTCommon-0.0.9.1/SIOTC/Operations.py
--rw-rw-rw-   0        0        0      443 2023-04-12 16:56:02.000000 SIOTCommon-0.0.9.1/SIOTC/__init__.py
--rw-rw-rw-   0        0        0     2291 2023-04-19 16:48:43.000000 SIOTCommon-0.0.9.1/SIOTC/helperhttps.py
-drwxrwxrwx   0        0        0        0 2023-04-19 16:50:21.169390 SIOTCommon-0.0.9.1/SIOTCommon.egg-info/
--rw-rw-rw-   0        0        0      341 2023-04-19 16:50:20.000000 SIOTCommon-0.0.9.1/SIOTCommon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-04-19 16:50:20.000000 SIOTCommon-0.0.9.1/SIOTCommon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 16:50:20.000000 SIOTCommon-0.0.9.1/SIOTCommon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      636 2023-04-19 16:50:20.000000 SIOTCommon-0.0.9.1/SIOTCommon.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-19 16:50:20.000000 SIOTCommon-0.0.9.1/SIOTCommon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 16:50:21.172391 SIOTCommon-0.0.9.1/setup.cfg
--rw-rw-rw-   0        0        0      583 2023-04-19 16:33:39.000000 SIOTCommon-0.0.9.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:15:01.853420 SIOTCommon-0.0.9.2/
+-rw-rw-rw-   0        0        0      341 2023-04-19 17:15:01.852419 SIOTCommon-0.0.9.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-04-11 20:29:38.000000 SIOTCommon-0.0.9.2/README.txt
+drwxrwxrwx   0        0        0        0 2023-04-19 17:15:01.825420 SIOTCommon-0.0.9.2/SIOTC/
+-rw-rw-rw-   0        0        0     1851 2023-04-19 16:34:13.000000 SIOTCommon-0.0.9.2/SIOTC/DatabaseLayer.py
+-rw-rw-rw-   0        0        0     6846 2023-04-19 15:57:38.000000 SIOTCommon-0.0.9.2/SIOTC/Operations.py
+-rw-rw-rw-   0        0        0      443 2023-04-12 16:56:02.000000 SIOTCommon-0.0.9.2/SIOTC/__init__.py
+-rw-rw-rw-   0        0        0     2284 2023-04-19 17:14:41.000000 SIOTCommon-0.0.9.2/SIOTC/helperhttps.py
+drwxrwxrwx   0        0        0        0 2023-04-19 17:15:01.850419 SIOTCommon-0.0.9.2/SIOTCommon.egg-info/
+-rw-rw-rw-   0        0        0      341 2023-04-19 17:15:01.000000 SIOTCommon-0.0.9.2/SIOTCommon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-04-19 17:15:01.000000 SIOTCommon-0.0.9.2/SIOTCommon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 17:15:01.000000 SIOTCommon-0.0.9.2/SIOTCommon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      636 2023-04-19 17:15:01.000000 SIOTCommon-0.0.9.2/SIOTCommon.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-19 17:15:01.000000 SIOTCommon-0.0.9.2/SIOTCommon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-19 17:15:01.854426 SIOTCommon-0.0.9.2/setup.cfg
+-rw-rw-rw-   0        0        0      583 2023-04-19 17:14:56.000000 SIOTCommon-0.0.9.2/setup.py
```

### Comparing `SIOTCommon-0.0.9.1/SIOTC/DatabaseLayer.py` & `SIOTCommon-0.0.9.2/SIOTC/DatabaseLayer.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9.1/SIOTC/Operations.py` & `SIOTCommon-0.0.9.2/SIOTC/Operations.py`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9.1/SIOTC/helperhttps.py` & `SIOTCommon-0.0.9.2/SIOTC/helperhttps.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 from flask import request, jsonify
 from functools import wraps
 from flask_jwt_extended import get_current_user
 from enum import Enum
-import Operations
+import SIOTC.Operations as op
 import re
 
-op = Operations
-
 # Checks what type of data is being sent and returns correct object
 def CheckContentType():
     content_type = request.headers.get('Content-Type')
     if content_type == 'application/json':
         print('Json Message received')
         return request.json
     elif 'text/' in content_type:
```

### Comparing `SIOTCommon-0.0.9.1/SIOTCommon.egg-info/requires.txt` & `SIOTCommon-0.0.9.2/SIOTCommon.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `SIOTCommon-0.0.9.1/setup.py` & `SIOTCommon-0.0.9.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='SIOTCommon',
-    version='0.0.9.1',
+    version='0.0.9.2',
     packages=find_packages(),
     install_requires=requirements,
     author='Anton Persson',
     author_email='Antonnilspersson@gmail.com',
     description='Common operations for sweiot microservices',
     url='https://github.com/AntonNPersson/SweIoTServices.git',
     classifiers=[
```


# Comparing `tmp/django-rest-framework-simplify-1.5.0.dev1.tar.gz` & `tmp/django-rest-framework-simplify-1.5.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-rest-framework-simplify-1.5.0.dev1.tar", last modified: Thu Dec 29 22:51:20 2022, max compression
+gzip compressed data, was "dist/django-rest-framework-simplify-1.5.1.dev1.tar", last modified: Wed Apr 19 00:12:01 2023, max compression
```

## Comparing `django-rest-framework-simplify-1.5.0.dev1.tar` & `django-rest-framework-simplify-1.5.1.dev1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-29 22:51:20.000000 django-rest-framework-simplify-1.5.0.dev1/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-29 22:51:20.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-29 22:51:20.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/services/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-12-29 22:51:20.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/services/sql_executor/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/services/sql_executor/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      127 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/services/sql_executor/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7001 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/services/sql_executor/service.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1205 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/services/sql_executor/tests.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/services/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      121 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/apps.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1619 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      538 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4178 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/fields.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8510 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/forms.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1404 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/helpers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5639 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/mapper.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15271 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/models.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15319 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/serializer.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      751 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/signature.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    43921 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/views.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      765 2022-12-29 22:50:55.000000 django-rest-framework-simplify-1.5.0.dev1/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      299 2022-12-29 22:51:20.000000 django-rest-framework-simplify-1.5.0.dev1/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:12:01.000000 django-rest-framework-simplify-1.5.1.dev1/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:12:01.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:12:01.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/services/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:12:01.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/services/sql_executor/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/services/sql_executor/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      127 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/services/sql_executor/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7001 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/services/sql_executor/service.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1205 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/services/sql_executor/tests.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/services/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      121 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/apps.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1619 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      538 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4178 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/fields.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8510 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/forms.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1404 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/helpers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     5639 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/mapper.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15271 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/models.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15319 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/serializer.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      751 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/signature.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    43921 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/views.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      765 2023-04-19 00:11:41.000000 django-rest-framework-simplify-1.5.1.dev1/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      299 2023-04-19 00:12:01.000000 django-rest-framework-simplify-1.5.1.dev1/PKG-INFO
```

### Comparing `django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/services/sql_executor/service.py` & `django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/services/sql_executor/service.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/services/sql_executor/tests.py` & `django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/services/sql_executor/tests.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/errors.py` & `django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/errors.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/exceptions.py` & `django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/fields.py` & `django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/fields.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/forms.py` & `django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/forms.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/helpers.py` & `django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/helpers.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/mapper.py` & `django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/mapper.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/models.py` & `django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/models.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/serializer.py` & `django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/serializer.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/signature.py` & `django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/signature.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-simplify-1.5.0.dev1/rest_framework_simplify/views.py` & `django-rest-framework-simplify-1.5.1.dev1/rest_framework_simplify/views.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-simplify-1.5.0.dev1/setup.py` & `django-rest-framework-simplify-1.5.1.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='django-rest-framework-simplify',
-    version='1.5.0.dev1',
+    version='1.5.1.dev1',
     description='Django Rest Framework Simplify',
     author='Skyler Cain',
     author_email='skylercain@gmail.com',
     url='https://github.com/Skylude/django-rest-framework-simplify',
     packages=['rest_framework_simplify', 'rest_framework_simplify.services', 'rest_framework_simplify.services.sql_executor'],
     install_requires=[
         'appdirs',
```


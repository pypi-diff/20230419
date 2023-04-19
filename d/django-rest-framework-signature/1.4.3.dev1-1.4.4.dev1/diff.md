# Comparing `tmp/django-rest-framework-signature-1.4.3.dev1.tar.gz` & `tmp/django-rest-framework-signature-1.4.4.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-rest-framework-signature-1.4.3.dev1.tar", last modified: Mon Feb 28 23:40:48 2022, max compression
+gzip compressed data, was "dist/django-rest-framework-signature-1.4.4.dev1.tar", last modified: Wed Apr 19 00:09:24 2023, max compression
```

## Comparing `django-rest-framework-signature-1.4.3.dev1.tar` & `django-rest-framework-signature-1.4.4.dev1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-28 23:40:48.000000 django-rest-framework-signature-1.4.3.dev1/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-28 23:40:48.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-02-28 23:40:48.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/models/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/models/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3061 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/models/mongo.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3921 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/models/relational.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      124 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/apps.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10680 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/authentication.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1903 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/backend.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      178 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/cognito_urls.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1170 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/cognito_views.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1441 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/errors.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      200 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    14803 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/helpers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1282 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/jwt_validator.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3211 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/serializers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6684 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/settings.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1673 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/tests.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      732 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/urls.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9253 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/views.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      465 2022-02-28 23:40:26.000000 django-rest-framework-signature-1.4.3.dev1/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      382 2022-02-28 23:40:48.000000 django-rest-framework-signature-1.4.3.dev1/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:09:24.000000 django-rest-framework-signature-1.4.4.dev1/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:09:24.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:09:24.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/models/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/models/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3061 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/models/mongo.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3921 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/models/relational.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      124 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/apps.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10680 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/authentication.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1903 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/backend.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      178 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/cognito_urls.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1170 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/cognito_views.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1441 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/errors.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      200 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    14803 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/helpers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1282 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/jwt_validator.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3211 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/serializers.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     6684 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/settings.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1673 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/tests.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      732 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/urls.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     9253 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/views.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      465 2023-04-19 00:09:00.000000 django-rest-framework-signature-1.4.4.dev1/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      382 2023-04-19 00:09:24.000000 django-rest-framework-signature-1.4.4.dev1/PKG-INFO
```

### Comparing `django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/models/mongo.py` & `django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/models/mongo.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/models/relational.py` & `django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/models/relational.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/authentication.py` & `django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/authentication.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/backend.py` & `django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/backend.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/cognito_views.py` & `django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/cognito_views.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/errors.py` & `django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/errors.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/helpers.py` & `django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/helpers.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/jwt_validator.py` & `django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/jwt_validator.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/serializers.py` & `django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/serializers.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/settings.py` & `django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/settings.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/tests.py` & `django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/tests.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/urls.py` & `django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/urls.py`

 * *Files identical despite different names*

### Comparing `django-rest-framework-signature-1.4.3.dev1/rest_framework_signature/views.py` & `django-rest-framework-signature-1.4.4.dev1/rest_framework_signature/views.py`

 * *Files identical despite different names*


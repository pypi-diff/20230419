# Comparing `tmp/django-sentry-secure-source-map-0.0.1.tar.gz` & `tmp/django-sentry-secure-source-map-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-sentry-secure-source-map-0.0.1.tar", last modified: Thu Apr 13 16:08:54 2023, max compression
+gzip compressed data, was "django-sentry-secure-source-map-0.1.0.tar", last modified: Wed Apr 19 12:09:38 2023, max compression
```

## Comparing `django-sentry-secure-source-map-0.0.1.tar` & `django-sentry-secure-source-map-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1823 2023-04-13 14:50:26.319911 django-sentry-secure-source-map-0.0.1/.gitignore
--rw-r--r--   0        0        0     1069 2023-04-13 14:42:09.701651 django-sentry-secure-source-map-0.0.1/LICENSE
--rw-r--r--   0        0        0       94 2023-04-13 16:02:37.604627 django-sentry-secure-source-map-0.0.1/README.md
--rwxr-xr-x   0        0        0      248 2023-04-13 14:54:40.964126 django-sentry-secure-source-map-0.0.1/manage.py
--rw-r--r--   0        0        0      955 2023-04-13 16:01:29.081001 django-sentry-secure-source-map-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       88 2023-04-13 16:04:20.391731 django-sentry-secure-source-map-0.0.1/src/sentry_secure_source_map/__init__.py
--rw-r--r--   0        0        0      785 2023-04-13 16:00:59.577542 django-sentry-secure-source-map-0.0.1/src/sentry_secure_source_map/middleware.py
--rw-r--r--   0        0        0      750 1970-01-01 00:00:00.000000 django-sentry-secure-source-map-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1205 2023-04-19 12:09:31.031296 django-sentry-secure-source-map-0.1.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      587 2023-04-19 12:09:31.031296 django-sentry-secure-source-map-0.1.0/.github/workflows/pypi.yml
+-rw-r--r--   0        0        0     1799 2023-04-19 12:09:31.031296 django-sentry-secure-source-map-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1069 2023-04-19 12:09:31.031296 django-sentry-secure-source-map-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1284 2023-04-19 12:09:31.031296 django-sentry-secure-source-map-0.1.0/README.md
+-rwxr-xr-x   0        0        0      248 2023-04-19 12:09:31.031296 django-sentry-secure-source-map-0.1.0/manage.py
+-rw-r--r--   0        0        0     1521 2023-04-19 12:09:31.031296 django-sentry-secure-source-map-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       88 2023-04-19 12:09:31.031296 django-sentry-secure-source-map-0.1.0/src/sentry_secure_source_map/__init__.py
+-rw-r--r--   0        0        0      867 2023-04-19 12:09:31.031296 django-sentry-secure-source-map-0.1.0/src/sentry_secure_source_map/middleware.py
+-rw-r--r--   0        0        0     2538 1970-01-01 00:00:00.000000 django-sentry-secure-source-map-0.1.0/PKG-INFO
```

### Comparing `django-sentry-secure-source-map-0.0.1/.gitignore` & `django-sentry-secure-source-map-0.1.0/.gitignore`

 * *Files 16% similar despite different names*

```diff
@@ -123,9 +123,7 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
-
-tests/collected-static
```

### Comparing `django-sentry-secure-source-map-0.0.1/LICENSE` & `django-sentry-secure-source-map-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-sentry-secure-source-map-0.0.1/pyproject.toml` & `django-sentry-secure-source-map-0.1.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django-sentry-secure-source-map"
-description = ""
+description = "A middleware to ensure only Sentry can access source maps"
 authors = [{name = "Torchbox", email = "tech@torchbox.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
-classifiers = ["License :: OSI Approved :: MIT License"]
+classifiers = [
+    "Environment :: Web Environment",
+    "Framework :: Django",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python",
+    "Topic :: Internet :: WWW/HTTP",
+    "Topic :: Software Development",
+]
 dynamic = ["version"]
 requires-python = ">=3.7"
 dependencies = [
     "Django>=3.0,<5.0",
 ]
 
 [project.optional-dependencies]
 test = [
     "pytest-cov==3.0.0",
-    "pytest-mock==3.8.2",
     "pytest-django==4.5.2",
     "pytest==7.1.2",
 ]
 lint = [
     "ruff==0.0.261",
     "black==23.3.0",
 ]
```

### Comparing `django-sentry-secure-source-map-0.0.1/src/sentry_secure_source_map/middleware.py` & `django-sentry-secure-source-map-0.1.0/src/sentry_secure_source_map/middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from django.conf import settings
 from django.core.exceptions import MiddlewareNotUsed
 from django.http import HttpResponseForbidden
 from django.utils.crypto import constant_time_compare
 
 
 class SentrySecureSourceMapMiddleware:
+    """
+    Only allow Sentry to access sourcemap files.
+    """
+
     def __init__(self, get_response):
-        if not settings.SENTRY_SECURITY_TOKEN:
+        if not getattr(settings, "SENTRY_SECURITY_TOKEN", ""):
             raise MiddlewareNotUsed
 
         self.get_response = get_response
 
     def __call__(self, request):
         if request.path.startswith(settings.STATIC_URL) and request.path.endswith(
             ".map"
```


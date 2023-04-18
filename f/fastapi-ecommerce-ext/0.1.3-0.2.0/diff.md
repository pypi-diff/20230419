# Comparing `tmp/fastapi_ecommerce_ext-0.1.3.tar.gz` & `tmp/fastapi_ecommerce_ext-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_ecommerce_ext-0.1.3.tar", last modified: Tue Apr 18 23:09:35 2023, max compression
+gzip compressed data, was "fastapi_ecommerce_ext-0.2.0.tar", last modified: Tue Apr 18 23:22:46 2023, max compression
```

## Comparing `fastapi_ecommerce_ext-0.1.3.tar` & `fastapi_ecommerce_ext-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 23:09:35.633847 fastapi_ecommerce_ext-0.1.3/
--rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      383 2023-04-18 23:09:35.633847 fastapi_ecommerce_ext-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 23:09:35.622849 fastapi_ecommerce_ext-0.1.3/fastapi_ecommerce_ext/
-drwxrwxrwx   0        0        0        0 2023-04-18 23:09:35.632851 fastapi_ecommerce_ext-0.1.3/fastapi_ecommerce_ext/logger/
--rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.1.3/fastapi_ecommerce_ext/logger/__init__.py
--rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.1.3/fastapi_ecommerce_ext/logger/configure.py
--rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.1.3/fastapi_ecommerce_ext/logger/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-18 23:09:35.630848 fastapi_ecommerce_ext-0.1.3/fastapi_ecommerce_ext.egg-info/
--rw-rw-rw-   0        0        0      383 2023-04-18 23:09:35.000000 fastapi_ecommerce_ext-0.1.3/fastapi_ecommerce_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-04-18 23:09:35.000000 fastapi_ecommerce_ext-0.1.3/fastapi_ecommerce_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 23:09:35.000000 fastapi_ecommerce_ext-0.1.3/fastapi_ecommerce_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-18 23:09:35.000000 fastapi_ecommerce_ext-0.1.3/fastapi_ecommerce_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-18 23:09:35.000000 fastapi_ecommerce_ext-0.1.3/fastapi_ecommerce_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-18 23:09:35.634847 fastapi_ecommerce_ext-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      567 2023-04-18 23:09:34.000000 fastapi_ecommerce_ext-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 23:22:46.830405 fastapi_ecommerce_ext-0.2.0/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      383 2023-04-18 23:22:46.830405 fastapi_ecommerce_ext-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 23:22:46.820413 fastapi_ecommerce_ext-0.2.0/fastapi_ecommerce_ext/
+drwxrwxrwx   0        0        0        0 2023-04-18 23:22:46.829405 fastapi_ecommerce_ext-0.2.0/fastapi_ecommerce_ext/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.2.0/fastapi_ecommerce_ext/logger/__init__.py
+-rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.2.0/fastapi_ecommerce_ext/logger/configure.py
+-rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.2.0/fastapi_ecommerce_ext/logger/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-18 23:22:46.827406 fastapi_ecommerce_ext-0.2.0/fastapi_ecommerce_ext.egg-info/
+-rw-rw-rw-   0        0        0      383 2023-04-18 23:22:46.000000 fastapi_ecommerce_ext-0.2.0/fastapi_ecommerce_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-04-18 23:22:46.000000 fastapi_ecommerce_ext-0.2.0/fastapi_ecommerce_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 23:22:46.000000 fastapi_ecommerce_ext-0.2.0/fastapi_ecommerce_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-18 23:22:46.000000 fastapi_ecommerce_ext-0.2.0/fastapi_ecommerce_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-18 23:22:46.000000 fastapi_ecommerce_ext-0.2.0/fastapi_ecommerce_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-18 23:22:46.831405 fastapi_ecommerce_ext-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-04-18 23:22:46.000000 fastapi_ecommerce_ext-0.2.0/setup.py
```

### Comparing `fastapi_ecommerce_ext-0.1.3/LICENSE.txt` & `fastapi_ecommerce_ext-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.1.3/fastapi_ecommerce_ext/logger/configure.py` & `fastapi_ecommerce_ext-0.2.0/fastapi_ecommerce_ext/logger/configure.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.1.3/fastapi_ecommerce_ext/logger/middleware.py` & `fastapi_ecommerce_ext-0.2.0/fastapi_ecommerce_ext/logger/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.1.3/setup.py` & `fastapi_ecommerce_ext-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dotenv import load_dotenv
 from setuptools import setup
 
 load_dotenv()
 
 package_name = 'fastapi_ecommerce_ext'
 url = f'{os.getenv("GIT_REPO")}/pypi/{package_name}'
-version = 'v0.1.3'
+version = 'v0.2.0'
 setup(
     name=package_name,
     version=version,
     packages=['fastapi_ecommerce_ext.logger'],
     install_requires=[
         'loguru',
         'starlette',
```


# Comparing `tmp/fastapi_ecommerce_ext-0.1.1.tar.gz` & `tmp/fastapi_ecommerce_ext-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_ecommerce_ext-0.1.1.tar", last modified: Tue Apr 18 22:57:17 2023, max compression
+gzip compressed data, was "fastapi_ecommerce_ext-0.1.2.tar", last modified: Tue Apr 18 23:00:47 2023, max compression
```

## Comparing `fastapi_ecommerce_ext-0.1.1.tar` & `fastapi_ecommerce_ext-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 22:57:17.351167 fastapi_ecommerce_ext-0.1.1/
--rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      383 2023-04-18 22:57:17.351167 fastapi_ecommerce_ext-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 22:57:17.341167 fastapi_ecommerce_ext-0.1.1/fastapi_ecommerce_ext/
-drwxrwxrwx   0        0        0        0 2023-04-18 22:57:17.351167 fastapi_ecommerce_ext-0.1.1/fastapi_ecommerce_ext/logger/
--rw-rw-rw-   0        0        0        0 2023-04-18 22:51:21.000000 fastapi_ecommerce_ext-0.1.1/fastapi_ecommerce_ext/logger/__init__.py
--rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.1.1/fastapi_ecommerce_ext/logger/logger.py
--rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.1.1/fastapi_ecommerce_ext/logger/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:57:17.348169 fastapi_ecommerce_ext-0.1.1/fastapi_ecommerce_ext.egg-info/
--rw-rw-rw-   0        0        0      383 2023-04-18 22:57:17.000000 fastapi_ecommerce_ext-0.1.1/fastapi_ecommerce_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-04-18 22:57:17.000000 fastapi_ecommerce_ext-0.1.1/fastapi_ecommerce_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 22:57:17.000000 fastapi_ecommerce_ext-0.1.1/fastapi_ecommerce_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-18 22:57:17.000000 fastapi_ecommerce_ext-0.1.1/fastapi_ecommerce_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-18 22:57:17.000000 fastapi_ecommerce_ext-0.1.1/fastapi_ecommerce_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-18 22:57:17.352167 fastapi_ecommerce_ext-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      567 2023-04-18 22:57:16.000000 fastapi_ecommerce_ext-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 23:00:47.063905 fastapi_ecommerce_ext-0.1.2/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      383 2023-04-18 23:00:47.063905 fastapi_ecommerce_ext-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 23:00:47.052905 fastapi_ecommerce_ext-0.1.2/fastapi_ecommerce_ext/
+drwxrwxrwx   0        0        0        0 2023-04-18 23:00:47.062905 fastapi_ecommerce_ext-0.1.2/fastapi_ecommerce_ext/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.1.2/fastapi_ecommerce_ext/logger/__init__.py
+-rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.1.2/fastapi_ecommerce_ext/logger/logger.py
+-rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.1.2/fastapi_ecommerce_ext/logger/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-18 23:00:47.060906 fastapi_ecommerce_ext-0.1.2/fastapi_ecommerce_ext.egg-info/
+-rw-rw-rw-   0        0        0      383 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.1.2/fastapi_ecommerce_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2023-04-18 23:00:47.000000 fastapi_ecommerce_ext-0.1.2/fastapi_ecommerce_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.1.2/fastapi_ecommerce_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.1.2/fastapi_ecommerce_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.1.2/fastapi_ecommerce_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-18 23:00:47.064904 fastapi_ecommerce_ext-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.1.2/setup.py
```

### Comparing `fastapi_ecommerce_ext-0.1.1/LICENSE.txt` & `fastapi_ecommerce_ext-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.1.1/fastapi_ecommerce_ext/logger/logger.py` & `fastapi_ecommerce_ext-0.1.2/fastapi_ecommerce_ext/logger/logger.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.1.1/fastapi_ecommerce_ext/logger/middleware.py` & `fastapi_ecommerce_ext-0.1.2/fastapi_ecommerce_ext/logger/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.1.1/setup.py` & `fastapi_ecommerce_ext-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dotenv import load_dotenv
 from setuptools import setup
 
 load_dotenv()
 
 package_name = 'fastapi_ecommerce_ext'
 url = f'{os.getenv("GIT_REPO")}/pypi/{package_name}'
-version = 'v0.1.1'
+version = 'v0.1.2'
 setup(
     name=package_name,
     version=version,
     packages=['fastapi_ecommerce_ext.logger'],
     install_requires=[
         'loguru',
         'starlette',
```


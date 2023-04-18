# Comparing `tmp/fastapi-ecommerce-ext-0.1.3.tar.gz` & `tmp/fastapi_ecommerce_ext-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-ecommerce-ext-0.1.3.tar", last modified: Tue Apr 18 22:40:08 2023, max compression
+gzip compressed data, was "fastapi_ecommerce_ext-0.1.4.tar", last modified: Tue Apr 18 22:45:43 2023, max compression
```

## Comparing `fastapi-ecommerce-ext-0.1.3.tar` & `fastapi_ecommerce_ext-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 22:40:08.532637 fastapi-ecommerce-ext-0.1.3/
--rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi-ecommerce-ext-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      383 2023-04-18 22:40:08.532637 fastapi-ecommerce-ext-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi-ecommerce-ext-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 22:40:08.529638 fastapi-ecommerce-ext-0.1.3/fastapi_ecommerce_ext.egg-info/
--rw-rw-rw-   0        0        0      383 2023-04-18 22:40:08.000000 fastapi-ecommerce-ext-0.1.3/fastapi_ecommerce_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-04-18 22:40:08.000000 fastapi-ecommerce-ext-0.1.3/fastapi_ecommerce_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 22:40:08.000000 fastapi-ecommerce-ext-0.1.3/fastapi_ecommerce_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-18 22:40:08.000000 fastapi-ecommerce-ext-0.1.3/fastapi_ecommerce_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 22:40:08.000000 fastapi-ecommerce-ext-0.1.3/fastapi_ecommerce_ext.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 22:40:08.531637 fastapi-ecommerce-ext-0.1.3/logger/
--rw-rw-rw-   0        0        0        0 2023-04-18 21:09:14.000000 fastapi-ecommerce-ext-0.1.3/logger/__init__.py
--rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi-ecommerce-ext-0.1.3/logger/logger.py
--rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi-ecommerce-ext-0.1.3/logger/middleware.py
--rw-rw-rw-   0        0        0       86 2023-04-18 22:40:08.533637 fastapi-ecommerce-ext-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      523 2023-04-18 22:40:07.000000 fastapi-ecommerce-ext-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:45:43.400164 fastapi_ecommerce_ext-0.1.4/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      383 2023-04-18 22:45:43.401146 fastapi_ecommerce_ext-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 22:45:43.397148 fastapi_ecommerce_ext-0.1.4/fastapi_ecommerce_ext.egg-info/
+-rw-rw-rw-   0        0        0      383 2023-04-18 22:45:43.000000 fastapi_ecommerce_ext-0.1.4/fastapi_ecommerce_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-04-18 22:45:43.000000 fastapi_ecommerce_ext-0.1.4/fastapi_ecommerce_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 22:45:43.000000 fastapi_ecommerce_ext-0.1.4/fastapi_ecommerce_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-18 22:45:43.000000 fastapi_ecommerce_ext-0.1.4/fastapi_ecommerce_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 22:45:43.000000 fastapi_ecommerce_ext-0.1.4/fastapi_ecommerce_ext.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 22:45:43.400164 fastapi_ecommerce_ext-0.1.4/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-18 21:09:14.000000 fastapi_ecommerce_ext-0.1.4/logger/__init__.py
+-rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.1.4/logger/logger.py
+-rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.1.4/logger/middleware.py
+-rw-rw-rw-   0        0        0       86 2023-04-18 22:45:43.401146 fastapi_ecommerce_ext-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      545 2023-04-18 22:45:41.000000 fastapi_ecommerce_ext-0.1.4/setup.py
```

### Comparing `fastapi-ecommerce-ext-0.1.3/LICENSE.txt` & `fastapi_ecommerce_ext-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi-ecommerce-ext-0.1.3/logger/logger.py` & `fastapi_ecommerce_ext-0.1.4/logger/logger.py`

 * *Files identical despite different names*

### Comparing `fastapi-ecommerce-ext-0.1.3/logger/middleware.py` & `fastapi_ecommerce_ext-0.1.4/logger/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi-ecommerce-ext-0.1.3/setup.py` & `fastapi_ecommerce_ext-0.1.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 
-from setuptools import setup
 from dotenv import load_dotenv
+from setuptools import setup
 
 load_dotenv()
 
-url = f'{os.getenv("GIT_REPO")}/pypi/fastapi-ecommerce-ext'
-version = 'v0.1.3'
+package_name = 'fastapi_ecommerce_ext'
+url = f'{os.getenv("GIT_REPO")}/pypi/{package_name}'
+version = 'v0.1.4'
 setup(
-    name='fastapi-ecommerce-ext',
+    name=package_name,
     version=version,
     packages=['logger'],
     install_requires=[
         'loguru',
         'starlette',
     ],
     url=url,
```


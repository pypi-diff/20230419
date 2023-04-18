# Comparing `tmp/fastapi-ecommerce-ext-0.1.1.tar.gz` & `tmp/fastapi-ecommerce-ext-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-ecommerce-ext-0.1.1.tar", last modified: Tue Apr 18 22:10:05 2023, max compression
+gzip compressed data, was "fastapi-ecommerce-ext-0.1.2.tar", last modified: Tue Apr 18 22:34:42 2023, max compression
```

## Comparing `fastapi-ecommerce-ext-0.1.1.tar` & `fastapi-ecommerce-ext-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 22:10:05.311457 fastapi-ecommerce-ext-0.1.1/
--rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi-ecommerce-ext-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      422 2023-04-18 22:10:05.311457 fastapi-ecommerce-ext-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi-ecommerce-ext-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 22:10:05.308466 fastapi-ecommerce-ext-0.1.1/fastapi_ecommerce_ext.egg-info/
--rw-rw-rw-   0        0        0      422 2023-04-18 22:10:05.000000 fastapi-ecommerce-ext-0.1.1/fastapi_ecommerce_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      321 2023-04-18 22:10:05.000000 fastapi-ecommerce-ext-0.1.1/fastapi_ecommerce_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 22:10:05.000000 fastapi-ecommerce-ext-0.1.1/fastapi_ecommerce_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-18 22:10:05.000000 fastapi-ecommerce-ext-0.1.1/fastapi_ecommerce_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-18 22:10:05.000000 fastapi-ecommerce-ext-0.1.1/fastapi_ecommerce_ext.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-18 22:10:05.310455 fastapi-ecommerce-ext-0.1.1/logger/
--rw-rw-rw-   0        0        0        0 2023-04-18 21:09:14.000000 fastapi-ecommerce-ext-0.1.1/logger/__init__.py
--rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi-ecommerce-ext-0.1.1/logger/logger.py
--rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi-ecommerce-ext-0.1.1/logger/middleware.py
--rw-rw-rw-   0        0        0       86 2023-04-18 22:10:05.312474 fastapi-ecommerce-ext-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      522 2023-04-18 22:09:43.000000 fastapi-ecommerce-ext-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:34:42.280839 fastapi-ecommerce-ext-0.1.2/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi-ecommerce-ext-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      383 2023-04-18 22:34:42.280839 fastapi-ecommerce-ext-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi-ecommerce-ext-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 22:34:42.277828 fastapi-ecommerce-ext-0.1.2/fastapi_ecommerce_ext.egg-info/
+-rw-rw-rw-   0        0        0      383 2023-04-18 22:34:42.000000 fastapi-ecommerce-ext-0.1.2/fastapi_ecommerce_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2023-04-18 22:34:42.000000 fastapi-ecommerce-ext-0.1.2/fastapi_ecommerce_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 22:34:42.000000 fastapi-ecommerce-ext-0.1.2/fastapi_ecommerce_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-18 22:34:42.000000 fastapi-ecommerce-ext-0.1.2/fastapi_ecommerce_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-18 22:34:42.000000 fastapi-ecommerce-ext-0.1.2/fastapi_ecommerce_ext.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 22:34:42.279828 fastapi-ecommerce-ext-0.1.2/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-18 21:09:14.000000 fastapi-ecommerce-ext-0.1.2/logger/__init__.py
+-rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi-ecommerce-ext-0.1.2/logger/logger.py
+-rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi-ecommerce-ext-0.1.2/logger/middleware.py
+-rw-rw-rw-   0        0        0       86 2023-04-18 22:34:42.280839 fastapi-ecommerce-ext-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      523 2023-04-18 22:34:40.000000 fastapi-ecommerce-ext-0.1.2/setup.py
```

### Comparing `fastapi-ecommerce-ext-0.1.1/LICENSE.txt` & `fastapi-ecommerce-ext-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi-ecommerce-ext-0.1.1/logger/logger.py` & `fastapi-ecommerce-ext-0.1.2/logger/logger.py`

 * *Files identical despite different names*

### Comparing `fastapi-ecommerce-ext-0.1.1/logger/middleware.py` & `fastapi-ecommerce-ext-0.1.2/logger/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi-ecommerce-ext-0.1.1/setup.py` & `fastapi-ecommerce-ext-0.1.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+import os
+
 from setuptools import setup
+from dotenv import load_dotenv
+
+load_dotenv()
 
-url = 'https://github.com/coolworld2049/fastapi-ecommerce/pypi/fastapi-ecommerce-ext'
-version = 'v0.1.1'
+url = f'{os.getenv("GIT_REPO")}/pypi/fastapi-ecommerce-ext'
+version = 'v0.1.2'
 setup(
     name='fastapi-ecommerce-ext',
     version=version,
     packages=['logger'],
     install_requires=[
         'loguru',
         'starlette',
     ],
     url=url,
     download_url=f'{url}-{version}.tar.gz',
     license='MIT',
-    author='coolworld2049',
-    author_email='coolworld2049@gmail.com',
+    author=os.getenv("GIT_USERNAME"),
     description='logging extension for fastapi-microservices'
 )
```


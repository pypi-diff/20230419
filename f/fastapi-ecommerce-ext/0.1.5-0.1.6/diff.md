# Comparing `tmp/fastapi_ecommerce_ext-0.1.5.tar.gz` & `tmp/fastapi_ecommerce_ext-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_ecommerce_ext-0.1.5.tar", last modified: Tue Apr 18 22:47:41 2023, max compression
+gzip compressed data, was "fastapi_ecommerce_ext-0.1.6.tar", last modified: Tue Apr 18 22:49:21 2023, max compression
```

## Comparing `fastapi_ecommerce_ext-0.1.5.tar` & `fastapi_ecommerce_ext-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 22:47:41.718829 fastapi_ecommerce_ext-0.1.5/
--rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      383 2023-04-18 22:47:41.718829 fastapi_ecommerce_ext-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 22:47:41.708828 fastapi_ecommerce_ext-0.1.5/fastapi_ecommerce_ext/
-drwxrwxrwx   0        0        0        0 2023-04-18 22:47:41.717827 fastapi_ecommerce_ext-0.1.5/fastapi_ecommerce_ext/logger/
--rw-rw-rw-   0        0        0        0 2023-04-18 21:09:14.000000 fastapi_ecommerce_ext-0.1.5/fastapi_ecommerce_ext/logger/__init__.py
--rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.1.5/fastapi_ecommerce_ext/logger/logger.py
--rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.1.5/fastapi_ecommerce_ext/logger/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-18 22:47:41.715827 fastapi_ecommerce_ext-0.1.5/fastapi_ecommerce_ext.egg-info/
--rw-rw-rw-   0        0        0      383 2023-04-18 22:47:41.000000 fastapi_ecommerce_ext-0.1.5/fastapi_ecommerce_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2023-04-18 22:47:41.000000 fastapi_ecommerce_ext-0.1.5/fastapi_ecommerce_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 22:47:41.000000 fastapi_ecommerce_ext-0.1.5/fastapi_ecommerce_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-18 22:47:41.000000 fastapi_ecommerce_ext-0.1.5/fastapi_ecommerce_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-18 22:47:41.000000 fastapi_ecommerce_ext-0.1.5/fastapi_ecommerce_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-18 22:47:41.719827 fastapi_ecommerce_ext-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      567 2023-04-18 22:46:52.000000 fastapi_ecommerce_ext-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:49:21.346229 fastapi_ecommerce_ext-0.1.6/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.1.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      383 2023-04-18 22:49:21.346229 fastapi_ecommerce_ext-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 22:49:21.339234 fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext/
+-rw-rw-rw-   0        0        0        0 2023-04-18 22:47:14.000000 fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:49:21.345228 fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-18 21:09:14.000000 fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext/logger/__init__.py
+-rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext/logger/logger.py
+-rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext/logger/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-18 22:49:21.343227 fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext.egg-info/
+-rw-rw-rw-   0        0        0      383 2023-04-18 22:49:21.000000 fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-04-18 22:49:21.000000 fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 22:49:21.000000 fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-18 22:49:21.000000 fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-18 22:49:21.000000 fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-04-18 22:49:21.347229 fastapi_ecommerce_ext-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      519 2023-04-18 22:49:19.000000 fastapi_ecommerce_ext-0.1.6/setup.py
```

### Comparing `fastapi_ecommerce_ext-0.1.5/LICENSE.txt` & `fastapi_ecommerce_ext-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.1.5/fastapi_ecommerce_ext/logger/logger.py` & `fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext/logger/logger.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.1.5/fastapi_ecommerce_ext/logger/middleware.py` & `fastapi_ecommerce_ext-0.1.6/fastapi_ecommerce_ext/logger/middleware.py`

 * *Files identical despite different names*


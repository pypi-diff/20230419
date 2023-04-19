# Comparing `tmp/fastapi_ecommerce_ext-0.2.2.tar.gz` & `tmp/fastapi_ecommerce_ext-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_ecommerce_ext-0.2.2.tar", last modified: Tue Apr 18 23:42:39 2023, max compression
+gzip compressed data, was "fastapi_ecommerce_ext-0.2.3.tar", last modified: Wed Apr 19 13:32:51 2023, max compression
```

## Comparing `fastapi_ecommerce_ext-0.2.2.tar` & `fastapi_ecommerce_ext-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 23:42:39.433043 fastapi_ecommerce_ext-0.2.2/
--rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.2.2/LICENSE.txt
--rw-rw-rw-   0        0        0      383 2023-04-18 23:42:39.434043 fastapi_ecommerce_ext-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 23:42:39.423043 fastapi_ecommerce_ext-0.2.2/fastapi_ecommerce_ext/
-drwxrwxrwx   0        0        0        0 2023-04-18 23:42:39.433043 fastapi_ecommerce_ext-0.2.2/fastapi_ecommerce_ext/logger/
--rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.2.2/fastapi_ecommerce_ext/logger/__init__.py
--rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.2.2/fastapi_ecommerce_ext/logger/configure.py
--rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.2.2/fastapi_ecommerce_ext/logger/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-18 23:42:39.430041 fastapi_ecommerce_ext-0.2.2/fastapi_ecommerce_ext.egg-info/
--rw-rw-rw-   0        0        0      383 2023-04-18 23:42:39.000000 fastapi_ecommerce_ext-0.2.2/fastapi_ecommerce_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-04-18 23:42:39.000000 fastapi_ecommerce_ext-0.2.2/fastapi_ecommerce_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 23:42:39.000000 fastapi_ecommerce_ext-0.2.2/fastapi_ecommerce_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-18 23:42:39.000000 fastapi_ecommerce_ext-0.2.2/fastapi_ecommerce_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-18 23:42:39.000000 fastapi_ecommerce_ext-0.2.2/fastapi_ecommerce_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-04-18 23:42:39.435043 fastapi_ecommerce_ext-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      535 2023-04-18 23:42:38.000000 fastapi_ecommerce_ext-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 13:32:51.367547 fastapi_ecommerce_ext-0.2.3/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.2.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      383 2023-04-19 13:32:51.367547 fastapi_ecommerce_ext-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 13:32:51.356660 fastapi_ecommerce_ext-0.2.3/fastapi_ecommerce_ext/
+drwxrwxrwx   0        0        0        0 2023-04-19 13:32:51.367547 fastapi_ecommerce_ext-0.2.3/fastapi_ecommerce_ext/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.2.3/fastapi_ecommerce_ext/logger/__init__.py
+-rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.2.3/fastapi_ecommerce_ext/logger/configure.py
+-rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.2.3/fastapi_ecommerce_ext/logger/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-19 13:32:51.367547 fastapi_ecommerce_ext-0.2.3/fastapi_ecommerce_ext.egg-info/
+-rw-rw-rw-   0        0        0      383 2023-04-19 13:32:51.000000 fastapi_ecommerce_ext-0.2.3/fastapi_ecommerce_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-04-19 13:32:51.000000 fastapi_ecommerce_ext-0.2.3/fastapi_ecommerce_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 13:32:51.000000 fastapi_ecommerce_ext-0.2.3/fastapi_ecommerce_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-19 13:32:51.000000 fastapi_ecommerce_ext-0.2.3/fastapi_ecommerce_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-19 13:32:51.000000 fastapi_ecommerce_ext-0.2.3/fastapi_ecommerce_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      142 2023-04-19 13:32:51.367547 fastapi_ecommerce_ext-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1092 2023-04-19 13:32:49.000000 fastapi_ecommerce_ext-0.2.3/setup.py
```

### Comparing `fastapi_ecommerce_ext-0.2.2/LICENSE.txt` & `fastapi_ecommerce_ext-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.2.2/fastapi_ecommerce_ext/logger/configure.py` & `fastapi_ecommerce_ext-0.2.3/fastapi_ecommerce_ext/logger/configure.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.2.2/fastapi_ecommerce_ext/logger/middleware.py` & `fastapi_ecommerce_ext-0.2.3/fastapi_ecommerce_ext/logger/middleware.py`

 * *Files identical despite different names*


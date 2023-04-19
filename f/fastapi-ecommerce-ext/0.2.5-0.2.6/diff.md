# Comparing `tmp/fastapi_ecommerce_ext-0.2.5.tar.gz` & `tmp/fastapi_ecommerce_ext-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_ecommerce_ext-0.2.5.tar", last modified: Wed Apr 19 15:54:28 2023, max compression
+gzip compressed data, was "fastapi_ecommerce_ext-0.2.6.tar", last modified: Wed Apr 19 15:55:58 2023, max compression
```

## Comparing `fastapi_ecommerce_ext-0.2.5.tar` & `fastapi_ecommerce_ext-0.2.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 15:54:28.324943 fastapi_ecommerce_ext-0.2.5/
--rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0      383 2023-04-19 15:54:28.325944 fastapi_ecommerce_ext-0.2.5/PKG-INFO
--rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 15:54:28.313946 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/
-drwxrwxrwx   0        0        0        0 2023-04-19 15:54:28.324943 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/logger/
--rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/logger/__init__.py
--rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/logger/configure.py
--rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/logger/middleware.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:54:28.322944 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext.egg-info/
--rw-rw-rw-   0        0        0      383 2023-04-19 15:54:28.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      390 2023-04-19 15:54:28.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 15:54:28.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-19 15:54:28.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-19 15:54:28.000000 fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      142 2023-04-19 15:54:28.326451 fastapi_ecommerce_ext-0.2.5/setup.cfg
--rw-rw-rw-   0        0        0     1170 2023-04-19 15:54:27.000000 fastapi_ecommerce_ext-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:55:58.389208 fastapi_ecommerce_ext-0.2.6/
+-rw-rw-rw-   0        0        0     1077 2023-04-18 21:58:50.000000 fastapi_ecommerce_ext-0.2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0      383 2023-04-19 15:55:58.389208 fastapi_ecommerce_ext-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2023-04-18 21:30:40.000000 fastapi_ecommerce_ext-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-19 15:55:58.379209 fastapi_ecommerce_ext-0.2.6/fastapi_ecommerce_ext/
+drwxrwxrwx   0        0        0        0 2023-04-19 15:55:58.388209 fastapi_ecommerce_ext-0.2.6/fastapi_ecommerce_ext/logger/
+-rw-rw-rw-   0        0        0        0 2023-04-18 23:00:46.000000 fastapi_ecommerce_ext-0.2.6/fastapi_ecommerce_ext/logger/__init__.py
+-rw-rw-rw-   0        0        0     1833 2023-04-13 22:35:53.000000 fastapi_ecommerce_ext-0.2.6/fastapi_ecommerce_ext/logger/configure.py
+-rw-rw-rw-   0        0        0     3016 2023-04-17 18:37:13.000000 fastapi_ecommerce_ext-0.2.6/fastapi_ecommerce_ext/logger/middleware.py
+drwxrwxrwx   0        0        0        0 2023-04-19 15:55:58.386209 fastapi_ecommerce_ext-0.2.6/fastapi_ecommerce_ext.egg-info/
+-rw-rw-rw-   0        0        0      383 2023-04-19 15:55:58.000000 fastapi_ecommerce_ext-0.2.6/fastapi_ecommerce_ext.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      390 2023-04-19 15:55:58.000000 fastapi_ecommerce_ext-0.2.6/fastapi_ecommerce_ext.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-19 15:55:58.000000 fastapi_ecommerce_ext-0.2.6/fastapi_ecommerce_ext.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-04-19 15:55:58.000000 fastapi_ecommerce_ext-0.2.6/fastapi_ecommerce_ext.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-04-19 15:55:58.000000 fastapi_ecommerce_ext-0.2.6/fastapi_ecommerce_ext.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      142 2023-04-19 15:55:58.390209 fastapi_ecommerce_ext-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1155 2023-04-19 15:55:56.000000 fastapi_ecommerce_ext-0.2.6/setup.py
```

### Comparing `fastapi_ecommerce_ext-0.2.5/LICENSE.txt` & `fastapi_ecommerce_ext-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/logger/configure.py` & `fastapi_ecommerce_ext-0.2.6/fastapi_ecommerce_ext/logger/configure.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.2.5/fastapi_ecommerce_ext/logger/middleware.py` & `fastapi_ecommerce_ext-0.2.6/fastapi_ecommerce_ext/logger/middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_ecommerce_ext-0.2.5/setup.py` & `fastapi_ecommerce_ext-0.2.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,22 @@
         from pip._internal.download import PipSession  # noqa
         from pip._internal.req import parse_requirements  # noqa
     except ImportError:
         # pip <= 9.0.3
         from pip.download import PipSession  # noqa
         from pip.req import parse_requirements  # noqa
 
-version = "v0.2.5"
+version = "v0.2.6"
 package_name = "fastapi_ecommerce_ext"
 url = f"https://github.com/coolworld2049/fastapi-ecommerce/pypi/{package_name}"
 
 install_requires = [
     str(x.requirement)
     for x in parse_requirements(
-        f"{package_name}/requirements.txt", PipSession()
+        f"requirements.txt", PipSession()
     )
 ]
 print(install_requires)
 setup(
     name=package_name,
     version=version,
     packages=["fastapi_ecommerce_ext.logger"],
```


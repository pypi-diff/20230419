# Comparing `tmp/globus-compute-sdk-2.0.1a2.tar.gz` & `tmp/globus-compute-sdk-2.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-sdk-2.0.1a2.tar", last modified: Tue Apr 18 21:51:09 2023, max compression
+gzip compressed data, was "globus-compute-sdk-2.0.1a3.tar", last modified: Tue Apr 18 22:05:54 2023, max compression
```

## Comparing `globus-compute-sdk-2.0.1a2.tar` & `globus-compute-sdk-2.0.1a3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:09.487183 globus-compute-sdk-2.0.1a2/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-18 19:39:56.000000 globus-compute-sdk-2.0.1a2/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1627 2023-04-18 21:51:09.487253 globus-compute-sdk-2.0.1a2/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      816 2023-04-18 19:39:56.000000 globus-compute-sdk-2.0.1a2/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:09.473866 globus-compute-sdk-2.0.1a2/globus_compute_sdk/
--rw-r--r--   0 lei        (501) staff       (20)      433 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:09.474930 globus-compute-sdk-2.0.1a2/globus_compute_sdk/errors/
--rw-r--r--   0 lei        (501) staff       (20)      320 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/errors/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1921 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/errors/error_types.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:09.476953 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      970 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/_environments.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:09.477499 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/asynchronous/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/asynchronous/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      648 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/asynchronous/compute_future.py
--rw-r--r--   0 lei        (501) staff       (20)      724 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/asynchronous/compute_task.py
--rw-r--r--   0 lei        (501) staff       (20)    11442 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
--rw-r--r--   0 lei        (501) staff       (20)     2262 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/batch.py
--rw-r--r--   0 lei        (501) staff       (20)    26362 2023-04-13 13:57:47.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/client.py
--rw-r--r--   0 lei        (501) staff       (20)     2400 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/container_spec.py
--rw-r--r--   0 lei        (501) staff       (20)    46344 2023-04-14 19:00:55.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/executor.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:09.485104 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/
--rw-r--r--   0 lei        (501) staff       (20)      237 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1787 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 lei        (501) staff       (20)      855 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 lei        (501) staff       (20)      373 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 lei        (501) staff       (20)      954 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 lei        (501) staff       (20)     7287 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 lei        (501) staff       (20)      710 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 lei        (501) staff       (20)     2887 2023-04-13 00:34:31.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/tokenstore.py
--rw-r--r--   0 lei        (501) staff       (20)     2190 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/whoami.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:09.485537 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/utils/
--rw-r--r--   0 lei        (501) staff       (20)      212 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1207 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/utils/printing.py
--rw-r--r--   0 lei        (501) staff       (20)     8618 2023-04-13 13:57:47.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/web_client.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:09.487030 globus-compute-sdk-2.0.1a2/globus_compute_sdk/serialize/
--rw-r--r--   0 lei        (501) staff       (20)      100 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/serialize/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1680 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/serialize/base.py
--rw-r--r--   0 lei        (501) staff       (20)     7511 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/serialize/concretes.py
--rw-r--r--   0 lei        (501) staff       (20)     3737 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/serialize/facade.py
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/utils.py
--rw-r--r--   0 lei        (501) staff       (20)      834 2023-04-18 21:17:41.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:09.474482 globus-compute-sdk-2.0.1a2/globus_compute_sdk.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1627 2023-04-18 21:51:09.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     1577 2023-04-18 21:51:09.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-18 21:51:09.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      397 2023-04-18 21:51:09.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       19 2023-04-18 21:51:09.000000 globus-compute-sdk-2.0.1a2/globus_compute_sdk.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-18 21:51:09.487583 globus-compute-sdk-2.0.1a2/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     2913 2023-04-18 19:39:56.000000 globus-compute-sdk-2.0.1a2/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:05:54.081889 globus-compute-sdk-2.0.1a3/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-18 19:39:56.000000 globus-compute-sdk-2.0.1a3/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1821 2023-04-18 22:05:54.081946 globus-compute-sdk-2.0.1a3/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      816 2023-04-18 19:39:56.000000 globus-compute-sdk-2.0.1a3/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:05:54.077739 globus-compute-sdk-2.0.1a3/globus_compute_sdk/
+-rw-r--r--   0 lei        (501) staff       (20)      433 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:05:54.078631 globus-compute-sdk-2.0.1a3/globus_compute_sdk/errors/
+-rw-r--r--   0 lei        (501) staff       (20)      320 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/errors/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1921 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/errors/error_types.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:05:54.079568 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      970 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/_environments.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:05:54.080056 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/asynchronous/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/asynchronous/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      648 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/asynchronous/compute_future.py
+-rw-r--r--   0 lei        (501) staff       (20)      724 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/asynchronous/compute_task.py
+-rw-r--r--   0 lei        (501) staff       (20)    11442 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
+-rw-r--r--   0 lei        (501) staff       (20)     2262 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/batch.py
+-rw-r--r--   0 lei        (501) staff       (20)    26362 2023-04-13 13:57:47.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/client.py
+-rw-r--r--   0 lei        (501) staff       (20)     2400 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/container_spec.py
+-rw-r--r--   0 lei        (501) staff       (20)    46344 2023-04-14 19:00:55.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/executor.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:05:54.081097 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/
+-rw-r--r--   0 lei        (501) staff       (20)      237 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1787 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/client_login.py
+-rw-r--r--   0 lei        (501) staff       (20)      855 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/decorators.py
+-rw-r--r--   0 lei        (501) staff       (20)      373 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/globus_auth.py
+-rw-r--r--   0 lei        (501) staff       (20)      954 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/login_flow.py
+-rw-r--r--   0 lei        (501) staff       (20)     7287 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)      710 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/protocol.py
+-rw-r--r--   0 lei        (501) staff       (20)     2887 2023-04-13 00:34:31.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/tokenstore.py
+-rw-r--r--   0 lei        (501) staff       (20)     2190 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/whoami.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:05:54.081336 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/utils/
+-rw-r--r--   0 lei        (501) staff       (20)      212 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1207 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/utils/printing.py
+-rw-r--r--   0 lei        (501) staff       (20)     8618 2023-04-13 13:57:47.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/web_client.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:05:54.081786 globus-compute-sdk-2.0.1a3/globus_compute_sdk/serialize/
+-rw-r--r--   0 lei        (501) staff       (20)      100 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/serialize/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1680 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/serialize/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     7511 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/serialize/concretes.py
+-rw-r--r--   0 lei        (501) staff       (20)     3737 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/serialize/facade.py
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/utils.py
+-rw-r--r--   0 lei        (501) staff       (20)      834 2023-04-18 22:04:14.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:05:54.078397 globus-compute-sdk-2.0.1a3/globus_compute_sdk.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1821 2023-04-18 22:05:54.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     1577 2023-04-18 22:05:54.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-18 22:05:54.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      397 2023-04-18 22:05:54.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       19 2023-04-18 22:05:54.000000 globus-compute-sdk-2.0.1a3/globus_compute_sdk.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-18 22:05:54.082228 globus-compute-sdk-2.0.1a3/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3161 2023-04-18 22:02:44.000000 globus-compute-sdk-2.0.1a3/setup.py
```

### Comparing `globus-compute-sdk-2.0.1a2/LICENSE` & `globus-compute-sdk-2.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/PKG-INFO` & `globus-compute-sdk-2.0.1a3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.0.1a2
+Version: 2.0.1a3
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
+Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
+Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `globus-compute-sdk-2.0.1a2/PyPI.md` & `globus-compute-sdk-2.0.1a3/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/errors/error_types.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/errors/error_types.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/_environments.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/_environments.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/asynchronous/compute_future.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/asynchronous/compute_future.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/asynchronous/compute_task.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/asynchronous/compute_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/batch.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/batch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/client.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/client.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/container_spec.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/container_spec.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/executor.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/client_login.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/decorators.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/login_flow.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/manager.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/protocol.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/tokenstore.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/login_manager/whoami.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/login_manager/whoami.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/utils/printing.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/utils/printing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/sdk/web_client.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/sdk/web_client.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/serialize/base.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/serialize/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/serialize/concretes.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/serialize/facade.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk/version.py` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.1a2"
+__version__ = "2.0.1a3"
 
 
 def compare_versions(
     current: str, min_version: str, *, package_name: str = "globus-compute-sdk"
 ) -> None:
     current_v = Version(current)
     min_v = Version(min_version)
```

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk.egg-info/PKG-INFO` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.0.1a2
+Version: 2.0.1a3
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
+Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
+Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `globus-compute-sdk-2.0.1a2/globus_compute_sdk.egg-info/SOURCES.txt` & `globus-compute-sdk-2.0.1a3/globus_compute_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.0.1a2/setup.py` & `globus-compute-sdk-2.0.1a3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,8 +88,12 @@
         "Topic :: Scientific/Engineering",
     ],
     keywords=["Globus Compute", "FaaS", "Function Serving"],
     author="Globus Compute Team",
     author_email="support@globus.org",
     license="Apache License, Version 2.0",
     url="https://github.com/funcx-faas/funcx",
+    project_urls={
+        "Changelog": "https://globus-compute.readthedocs.io/en/latest/changelog.html",  # noqa: E501
+        "Upgrade to Globus Compute": "https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html",  # noqa: E501
+    },
 )
```


# Comparing `tmp/funcx-endpoint-2.0.1a1.tar.gz` & `tmp/funcx-endpoint-2.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcx-endpoint-2.0.1a1.tar", last modified: Mon Apr 17 19:13:52 2023, max compression
+gzip compressed data, was "funcx-endpoint-2.0.1a2.tar", last modified: Tue Apr 18 22:00:03 2023, max compression
```

## Comparing `funcx-endpoint-2.0.1a1.tar` & `funcx-endpoint-2.0.1a2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:52.117795 funcx-endpoint-2.0.1a1/
--rw-r--r--   0 chris      (501) staff       (20)    11330 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.1a1/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)       16 2023-04-17 19:06:42.000000 funcx-endpoint-2.0.1a1/MANIFEST.in
--rw-r--r--   0 chris      (501) staff       (20)     1842 2023-04-17 19:13:52.117871 funcx-endpoint-2.0.1a1/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     1115 2023-04-17 18:38:33.000000 funcx-endpoint-2.0.1a1/PyPI.md
--rw-r--r--   0 chris      (501) staff       (20)      430 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.1a1/README.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:52.116448 funcx-endpoint-2.0.1a1/funcx_endpoint/
--rw-r--r--   0 chris      (501) staff       (20)      122 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.1a1/funcx_endpoint/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:52.117581 funcx-endpoint-2.0.1a1/funcx_endpoint/executors/
--rw-r--r--   0 chris      (501) staff       (20)      107 2023-04-12 14:51:48.000000 funcx-endpoint-2.0.1a1/funcx_endpoint/executors/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      245 2023-04-17 19:06:42.000000 funcx-endpoint-2.0.1a1/funcx_endpoint/version.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:13:52.117431 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     1842 2023-04-17 19:13:52.000000 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      376 2023-04-17 19:13:52.000000 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-04-17 19:13:52.000000 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)      329 2023-04-17 19:13:52.000000 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 chris      (501) staff       (20)       31 2023-04-17 19:13:52.000000 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       15 2023-04-17 19:13:52.000000 funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)      305 2023-04-17 19:13:52.118203 funcx-endpoint-2.0.1a1/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)     1776 2023-04-17 18:38:33.000000 funcx-endpoint-2.0.1a1/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:00:03.648461 funcx-endpoint-2.0.1a2/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a2/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-18 19:39:56.000000 funcx-endpoint-2.0.1a2/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     2042 2023-04-18 22:00:03.648514 funcx-endpoint-2.0.1a2/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     1115 2023-04-18 19:39:56.000000 funcx-endpoint-2.0.1a2/PyPI.md
+-rw-r--r--   0 lei        (501) staff       (20)      430 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a2/README.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:00:03.647535 funcx-endpoint-2.0.1a2/funcx_endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)      122 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a2/funcx_endpoint/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:00:03.648360 funcx-endpoint-2.0.1a2/funcx_endpoint/executors/
+-rw-r--r--   0 lei        (501) staff       (20)      107 2023-04-10 19:02:41.000000 funcx-endpoint-2.0.1a2/funcx_endpoint/executors/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      245 2023-04-18 21:17:41.000000 funcx-endpoint-2.0.1a2/funcx_endpoint/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:00:03.648246 funcx-endpoint-2.0.1a2/funcx_endpoint.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     2042 2023-04-18 22:00:03.000000 funcx-endpoint-2.0.1a2/funcx_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      376 2023-04-18 22:00:03.000000 funcx-endpoint-2.0.1a2/funcx_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-18 22:00:03.000000 funcx-endpoint-2.0.1a2/funcx_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      329 2023-04-18 22:00:03.000000 funcx-endpoint-2.0.1a2/funcx_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 lei        (501) staff       (20)       33 2023-04-18 22:00:03.000000 funcx-endpoint-2.0.1a2/funcx_endpoint.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       15 2023-04-18 22:00:03.000000 funcx-endpoint-2.0.1a2/funcx_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      305 2023-04-18 22:00:03.648732 funcx-endpoint-2.0.1a2/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     2032 2023-04-18 21:59:27.000000 funcx-endpoint-2.0.1a2/setup.py
```

### Comparing `funcx-endpoint-2.0.1a1/LICENSE` & `funcx-endpoint-2.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `funcx-endpoint-2.0.1a1/PKG-INFO` & `funcx-endpoint-2.0.1a2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: funcx-endpoint
-Version: 2.0.1a1
+Version: 2.0.1a2
 Summary: funcX: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
+Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
+Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
 Keywords: funcX,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -22,10 +24,10 @@
 
 This package is deprecated, and currently just wraps the [Globus Compute Endpoint](https://pypi.org/project/globus-compute-endpoint/) package with funcX names. See [here](https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html) for instructions on how to upgrade.
 
 # funcX Endpoint
 
 [funcX](https://globus-compute.readthedocs.io/en/latest/) is a distributed Function as a Service (FaaS) platform that enables flexible, scalable, and high performance remote function execution. Unlike centralized FaaS platforms, funcX allows users to execute functions on heterogeneous remote computers, from laptops to campus clusters, clouds, and supercomputers.
 
-This package provides the [funcX Endpoint](https://globus-compute.readthedocs.io/en/latest/endpoints.html) agent — the software which recieves user-submitted tasks (functions + arguments) and manages their execution on target machines — in addition to command line tools for managing funcX endpoints.
+This package provides the [funcX Endpoint](https://globus-compute.readthedocs.io/en/latest/endpoints.html) agent — the software which receives user-submitted tasks (functions + arguments) and manages their execution on target machines — in addition to command line tools for managing funcX endpoints.
 
 To submit functions for execution on funcX endpoints, use the companion [funcX SDK](https://pypi.org/project/funcx/) package.
```

### Comparing `funcx-endpoint-2.0.1a1/PyPI.md` & `funcx-endpoint-2.0.1a2/PyPI.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,10 +2,10 @@
 
 This package is deprecated, and currently just wraps the [Globus Compute Endpoint](https://pypi.org/project/globus-compute-endpoint/) package with funcX names. See [here](https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html) for instructions on how to upgrade.
 
 # funcX Endpoint
 
 [funcX](https://globus-compute.readthedocs.io/en/latest/) is a distributed Function as a Service (FaaS) platform that enables flexible, scalable, and high performance remote function execution. Unlike centralized FaaS platforms, funcX allows users to execute functions on heterogeneous remote computers, from laptops to campus clusters, clouds, and supercomputers.
 
-This package provides the [funcX Endpoint](https://globus-compute.readthedocs.io/en/latest/endpoints.html) agent — the software which recieves user-submitted tasks (functions + arguments) and manages their execution on target machines — in addition to command line tools for managing funcX endpoints.
+This package provides the [funcX Endpoint](https://globus-compute.readthedocs.io/en/latest/endpoints.html) agent — the software which receives user-submitted tasks (functions + arguments) and manages their execution on target machines — in addition to command line tools for managing funcX endpoints.
 
 To submit functions for execution on funcX endpoints, use the companion [funcX SDK](https://pypi.org/project/funcx/) package.
```

### Comparing `funcx-endpoint-2.0.1a1/funcx_endpoint.egg-info/PKG-INFO` & `funcx-endpoint-2.0.1a2/funcx_endpoint.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: funcx-endpoint
-Version: 2.0.1a1
+Version: 2.0.1a2
 Summary: funcX: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
+Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
+Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
 Keywords: funcX,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -22,10 +24,10 @@
 
 This package is deprecated, and currently just wraps the [Globus Compute Endpoint](https://pypi.org/project/globus-compute-endpoint/) package with funcX names. See [here](https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html) for instructions on how to upgrade.
 
 # funcX Endpoint
 
 [funcX](https://globus-compute.readthedocs.io/en/latest/) is a distributed Function as a Service (FaaS) platform that enables flexible, scalable, and high performance remote function execution. Unlike centralized FaaS platforms, funcX allows users to execute functions on heterogeneous remote computers, from laptops to campus clusters, clouds, and supercomputers.
 
-This package provides the [funcX Endpoint](https://globus-compute.readthedocs.io/en/latest/endpoints.html) agent — the software which recieves user-submitted tasks (functions + arguments) and manages their execution on target machines — in addition to command line tools for managing funcX endpoints.
+This package provides the [funcX Endpoint](https://globus-compute.readthedocs.io/en/latest/endpoints.html) agent — the software which receives user-submitted tasks (functions + arguments) and manages their execution on target machines — in addition to command line tools for managing funcX endpoints.
 
 To submit functions for execution on funcX endpoints, use the companion [funcX SDK](https://pypi.org/project/funcx/) package.
```

### Comparing `funcx-endpoint-2.0.1a1/setup.py` & `funcx-endpoint-2.0.1a2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
-    "globus-compute-endpoint>=2.0.0",
+    "globus-compute-endpoint>=2.0.1a2",
 ]
 
 version_ns = {}
 with open(os.path.join("funcx_endpoint", "version.py")) as f:
     exec(f.read(), version_ns)
 version = version_ns["__version__"]
 
@@ -47,8 +47,12 @@
         ]
     },
     include_package_data=True,
     author="Globus Compute Team",
     author_email="support@globus.org",
     license="Apache License, Version 2.0",
     url="https://github.com/funcx-faas/funcx",
+    project_urls={
+        "Changelog": "https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html",  # noqa: E501
+        "Upgrade to Globus Compute": "https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html",  # noqa: E501
+    },
 )
```


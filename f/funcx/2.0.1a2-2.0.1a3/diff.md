# Comparing `tmp/funcx-2.0.1a2.tar.gz` & `tmp/funcx-2.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcx-2.0.1a2.tar", last modified: Tue Apr 18 21:56:05 2023, max compression
+gzip compressed data, was "funcx-2.0.1a3.tar", last modified: Tue Apr 18 22:07:33 2023, max compression
```

## Comparing `funcx-2.0.1a2.tar` & `funcx-2.0.1a3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:56:05.840100 funcx-2.0.1a2/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 funcx-2.0.1a2/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-18 19:39:56.000000 funcx-2.0.1a2/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     2058 2023-04-18 21:56:05.840148 funcx-2.0.1a2/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     1051 2023-04-18 19:39:56.000000 funcx-2.0.1a2/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:56:05.839213 funcx-2.0.1a2/funcx/
--rw-r--r--   0 lei        (501) staff       (20)      467 2023-04-10 19:02:41.000000 funcx-2.0.1a2/funcx/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:56:05.839949 funcx-2.0.1a2/funcx/serialize/
--rw-r--r--   0 lei        (501) staff       (20)      110 2023-04-10 19:02:41.000000 funcx-2.0.1a2/funcx/serialize/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1146 2023-04-18 21:17:41.000000 funcx-2.0.1a2/funcx/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:56:05.839827 funcx-2.0.1a2/funcx.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     2058 2023-04-18 21:56:05.000000 funcx-2.0.1a2/funcx.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      253 2023-04-18 21:56:05.000000 funcx-2.0.1a2/funcx.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-18 21:56:05.000000 funcx-2.0.1a2/funcx.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)       28 2023-04-18 21:56:05.000000 funcx-2.0.1a2/funcx.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)        6 2023-04-18 21:56:05.000000 funcx-2.0.1a2/funcx.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      305 2023-04-18 21:56:05.840374 funcx-2.0.1a2/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     1976 2023-04-18 21:17:41.000000 funcx-2.0.1a2/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:07:33.489418 funcx-2.0.1a3/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 funcx-2.0.1a3/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-18 19:39:56.000000 funcx-2.0.1a3/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1997 2023-04-18 22:07:33.489464 funcx-2.0.1a3/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     1051 2023-04-18 19:39:56.000000 funcx-2.0.1a3/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:07:33.488628 funcx-2.0.1a3/funcx/
+-rw-r--r--   0 lei        (501) staff       (20)      467 2023-04-10 19:02:41.000000 funcx-2.0.1a3/funcx/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:07:33.489307 funcx-2.0.1a3/funcx/serialize/
+-rw-r--r--   0 lei        (501) staff       (20)      110 2023-04-10 19:02:41.000000 funcx-2.0.1a3/funcx/serialize/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     1146 2023-04-18 22:04:28.000000 funcx-2.0.1a3/funcx/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 22:07:33.489196 funcx-2.0.1a3/funcx.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1997 2023-04-18 22:07:33.000000 funcx-2.0.1a3/funcx.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      253 2023-04-18 22:07:33.000000 funcx-2.0.1a3/funcx.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-18 22:07:33.000000 funcx-2.0.1a3/funcx.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)       28 2023-04-18 22:07:33.000000 funcx-2.0.1a3/funcx.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)        6 2023-04-18 22:07:33.000000 funcx-2.0.1a3/funcx.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      305 2023-04-18 22:07:33.489678 funcx-2.0.1a3/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     1915 2023-04-18 22:04:23.000000 funcx-2.0.1a3/setup.py
```

### Comparing `funcx-2.0.1a2/LICENSE` & `funcx-2.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `funcx-2.0.1a2/PKG-INFO` & `funcx-2.0.1a3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: funcx
-Version: 2.0.1a2
+Version: 2.0.1a3
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: The Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
-Project-URL: Source, https://github.com/funcx-faas/funcX
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
-Project-URL: Upgrade to globus-compute-sdk, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
+Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
 Keywords: funcX,FaaS,Function Serving,Globus Compute
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `funcx-2.0.1a2/PyPI.md` & `funcx-2.0.1a3/PyPI.md`

 * *Files identical despite different names*

### Comparing `funcx-2.0.1a2/funcx/version.py` & `funcx-2.0.1a3/funcx/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.1a2"
+__version__ = "2.0.1a3"
 
 DEPRECATION_FUNCX = """
 The funcX SDK has been renamed to Globus Compute SDK and the new package is
 available on PyPI:
     https://pypi.org/project/globus-compute-sdk/
 
 Please consider upgrading to Globus Compute.  More information can be found at:
```

### Comparing `funcx-2.0.1a2/funcx.egg-info/PKG-INFO` & `funcx-2.0.1a3/funcx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: funcx
-Version: 2.0.1a2
+Version: 2.0.1a3
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: The Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
-Project-URL: Source, https://github.com/funcx-faas/funcX
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html
-Project-URL: Upgrade to globus-compute-sdk, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
+Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
 Keywords: funcX,FaaS,Function Serving,Globus Compute
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

### Comparing `funcx-2.0.1a2/setup.py` & `funcx-2.0.1a3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import re
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
-    "globus-compute-sdk>=2.0.1a2",
+    "globus-compute-sdk>=2.0.1a3",
 ]
 
 
 def parse_version():
     # single source of truth for package version
     version_string = ""
     version_pattern = re.compile(r'__version__ = "([^"]*)"')
@@ -49,12 +49,11 @@
     ],
     keywords=["funcX", "FaaS", "Function Serving", "Globus Compute"],
     author="The Globus Compute Team",
     author_email="support@globus.org",
     license="Apache License, Version 2.0",
     url="https://github.com/funcx-faas/funcx",
     project_urls={
-        "Source": "https://github.com/funcx-faas/funcX",
         "Changelog": "https://globus-compute.readthedocs.io/en/latest/changelog_funcx.html",  # noqa: E501
-        "Upgrade to globus-compute-sdk": "https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html",  # noqa: E501
+        "Upgrade to Globus Compute": "https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html",  # noqa: E501
     },
 )
```


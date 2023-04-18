# Comparing `tmp/jupyverse_api-0.1.3.tar.gz` & `tmp/jupyverse_api-0.1.4.tar.gz`

## Comparing `jupyverse_api-0.1.3.tar` & `jupyverse_api-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,28 @@
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/__init__.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/py.typed
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/README.md
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      884 2020-02-02 00:00:00.000000 jupyverse_api-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     4918 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/retrolab/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/README.md
+-rw-r--r--   0        0        0     1371 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 jupyverse_api-0.1.4/PKG-INFO
```

### Comparing `jupyverse_api-0.1.3/jupyverse_api/__init__.py` & `jupyverse_api-0.1.4/jupyverse_api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
 from pydantic import BaseModel, Extra
 
 from .app import App
 
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse_api-0.1.3/jupyverse_api/app/__init__.py` & `jupyverse_api-0.1.4/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.3/jupyverse_api/auth/__init__.py` & `jupyverse_api-0.1.4/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.3/jupyverse_api/kernels/models.py` & `jupyverse_api-0.1.4/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.3/jupyverse_api/main/__init__.py` & `jupyverse_api-0.1.4/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.3/.gitignore` & `jupyverse_api-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.3/COPYING.md` & `jupyverse_api-0.1.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.1.3/pyproject.toml` & `jupyverse_api-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -21,22 +21,29 @@
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "pydantic >=1.10.6,<2",
+  "fastapi >=0.95.0,<1",
+  "rich-click >=1.6.1,<2",
+  "asphalt >=4.11.0,<5",
+  "asphalt-web[fastapi] >=1.1.0,<2",
 ]
 dynamic = ["version"]
 
 [project.license]
 text = "BSD 3-Clause License"
 
 [project.urls]
-Source = "https://github.com/jupyter-server/jupyverse/api"
+Source = "https://github.com/jupyter-server/jupyverse/jupyverse_api"
+
+[project.scripts]
+jupyverse = "jupyverse_api.cli:main"
 
 [project.entry-points."asphalt.components"]
 app = "jupyverse_api.main:AppComponent"
 jupyverse = "jupyverse_api.main:JupyverseComponent"
 
 [project.entry-points."jupyverse.components"]
 app = "jupyverse_api.main:AppComponent"
```

### Comparing `jupyverse_api-0.1.3/PKG-INFO` & `jupyverse_api-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: jupyverse_api
-Version: 0.1.3
+Version: 0.1.4
 Summary: The public API for Jupyverse
-Project-URL: Source, https://github.com/jupyter-server/jupyverse/api
+Project-URL: Source, https://github.com/jupyter-server/jupyverse/jupyverse_api
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: api,jupyverse
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
+Requires-Dist: asphalt-web[fastapi]<2,>=1.1.0
+Requires-Dist: asphalt<5,>=4.11.0
+Requires-Dist: fastapi<1,>=0.95.0
 Requires-Dist: pydantic<2,>=1.10.6
+Requires-Dist: rich-click<2,>=1.6.1
 Description-Content-Type: text/markdown
 
 # Jupyverse API
 
 The public API for Jupyverse.
```


# Comparing `tmp/raclients-3.1.3.tar.gz` & `tmp/raclients-3.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raclients-3.1.3.tar", max compression
+gzip compressed data, was "raclients-3.1.4.tar", max compression
```

## Comparing `raclients-3.1.3.tar` & `raclients-3.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0        0        0        0 2023-04-14 23:15:33.026518 raclients-3.1.3/LICENSES/
--rw-r--r--   0        0        0     1039 2023-04-14 23:15:33.026518 raclients-3.1.3/README.md
--rw-r--r--   0        0        0     1054 2023-04-14 23:15:34.236638 raclients-3.1.3/pyproject.toml
--rw-r--r--   0        0        0      300 2023-04-14 23:15:33.028518 raclients-3.1.3/raclients/__init__.py
--rw-r--r--   0        0        0     6858 2023-04-14 23:15:33.028518 raclients-3.1.3/raclients/auth.py
--rw-r--r--   0        0        0       99 2023-04-14 23:15:33.028518 raclients-3.1.3/raclients/graph/__init__.py
--rw-r--r--   0        0        0     7259 2023-04-14 23:15:33.028518 raclients-3.1.3/raclients/graph/client.py
--rw-r--r--   0        0        0     9291 2023-04-14 23:15:33.028518 raclients-3.1.3/raclients/graph/transport.py
--rw-r--r--   0        0        0     3105 2023-04-14 23:15:33.029518 raclients-3.1.3/raclients/graph/util.py
--rw-r--r--   0        0        0       99 2023-04-14 23:15:33.029518 raclients-3.1.3/raclients/modelclient/__init__.py
--rw-r--r--   0        0        0     4356 2023-04-14 23:15:33.029518 raclients-3.1.3/raclients/modelclient/base.py
--rw-r--r--   0        0        0     1940 2023-04-14 23:15:33.029518 raclients-3.1.3/raclients/modelclient/lora.py
--rw-r--r--   0        0        0     5320 2023-04-14 23:15:33.029518 raclients-3.1.3/raclients/modelclient/mo.py
--rw-r--r--   0        0        0        0 2023-04-14 23:15:33.072522 raclients-3.1.3/raclients/py.typed
--rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 raclients-3.1.3/PKG-INFO
+drwxr-xr-x   0        0        0        0 2023-04-19 14:33:30.773737 raclients-3.1.4/LICENSES/
+-rw-r--r--   0        0        0     1039 2023-04-19 14:33:30.773737 raclients-3.1.4/README.md
+-rw-r--r--   0        0        0     1063 2023-04-19 14:33:32.896855 raclients-3.1.4/pyproject.toml
+-rw-r--r--   0        0        0      300 2023-04-19 14:33:30.775737 raclients-3.1.4/raclients/__init__.py
+-rw-r--r--   0        0        0     6858 2023-04-19 14:33:30.775737 raclients-3.1.4/raclients/auth.py
+-rw-r--r--   0        0        0       99 2023-04-19 14:33:30.776737 raclients-3.1.4/raclients/graph/__init__.py
+-rw-r--r--   0        0        0     7259 2023-04-19 14:33:30.776737 raclients-3.1.4/raclients/graph/client.py
+-rw-r--r--   0        0        0     9291 2023-04-19 14:33:30.776737 raclients-3.1.4/raclients/graph/transport.py
+-rw-r--r--   0        0        0     3105 2023-04-19 14:33:30.776737 raclients-3.1.4/raclients/graph/util.py
+-rw-r--r--   0        0        0       99 2023-04-19 14:33:30.776737 raclients-3.1.4/raclients/modelclient/__init__.py
+-rw-r--r--   0        0        0     4356 2023-04-19 14:33:30.777737 raclients-3.1.4/raclients/modelclient/base.py
+-rw-r--r--   0        0        0     1940 2023-04-19 14:33:30.777737 raclients-3.1.4/raclients/modelclient/lora.py
+-rw-r--r--   0        0        0     5320 2023-04-19 14:33:30.777737 raclients-3.1.4/raclients/modelclient/mo.py
+-rw-r--r--   0        0        0        0 2023-04-19 14:33:30.821740 raclients-3.1.4/raclients/py.typed
+-rw-r--r--   0        0        0     1976 1970-01-01 00:00:00.000000 raclients-3.1.4/PKG-INFO
```

### Comparing `raclients-3.1.3/README.md` & `raclients-3.1.4/README.md`

 * *Files identical despite different names*

### Comparing `raclients-3.1.3/pyproject.toml` & `raclients-3.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raclients"
-version = "3.1.3"
+version = "3.1.4"
 description = "Clients for OS2mo/LoRa"
 authors = ["Magenta <info@magenta.dk>"]
 license = "MPL-2.0"
 readme = "README.md"
 homepage = "https://magenta.dk/"
 repository = "https://git.magenta.dk/rammearkitektur/ra-clients"
 keywords = ["os2mo", "lora"]
@@ -17,15 +17,15 @@
 fastapi = ">=0.88,<1.0"
 httpx = ">=0.23.3,<0.25.0"
 Authlib = "^1.2.0"
 gql = "^3.4.0"
 structlog = ">=22.3,<24.0"
 tenacity = "^8.2.2"
 more-itertools = "^9.1.0"
-ramodels = "^18.5.2"
+ramodels = ">=18.5.2,<20.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 pytest-asyncio = "^0.18.3"
 pre-commit = "^2.19.0"
 respx = "^0.20.1"
 pytest-cov = "^3.0.0"
```

### Comparing `raclients-3.1.3/raclients/auth.py` & `raclients-3.1.4/raclients/auth.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.3/raclients/graph/client.py` & `raclients-3.1.4/raclients/graph/client.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.3/raclients/graph/transport.py` & `raclients-3.1.4/raclients/graph/transport.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.3/raclients/graph/util.py` & `raclients-3.1.4/raclients/graph/util.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.3/raclients/modelclient/base.py` & `raclients-3.1.4/raclients/modelclient/base.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.3/raclients/modelclient/lora.py` & `raclients-3.1.4/raclients/modelclient/lora.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.3/raclients/modelclient/mo.py` & `raclients-3.1.4/raclients/modelclient/mo.py`

 * *Files identical despite different names*

### Comparing `raclients-3.1.3/PKG-INFO` & `raclients-3.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raclients
-Version: 3.1.3
+Version: 3.1.4
 Summary: Clients for OS2mo/LoRa
 Home-page: https://magenta.dk/
 License: MPL-2.0
 Keywords: os2mo,lora
 Author: Magenta
 Author-email: info@magenta.dk
 Requires-Python: >=3.10,<4.0
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Authlib (>=1.2.0,<2.0.0)
 Requires-Dist: fastapi (>=0.88,<1.0)
 Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: httpx (>=0.23.3,<0.25.0)
 Requires-Dist: more-itertools (>=9.1.0,<10.0.0)
 Requires-Dist: pydantic (>=1.10.5,<2.0.0)
-Requires-Dist: ramodels (>=18.5.2,<19.0.0)
+Requires-Dist: ramodels (>=18.5.2,<20.0.0)
 Requires-Dist: structlog (>=22.3,<24.0)
 Requires-Dist: tenacity (>=8.2.2,<9.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Repository, https://git.magenta.dk/rammearkitektur/ra-clients
 Description-Content-Type: text/markdown
 
 <!--
```


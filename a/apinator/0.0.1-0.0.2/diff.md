# Comparing `tmp/apinator-0.0.1.tar.gz` & `tmp/apinator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apinator-0.0.1.tar", last modified: Tue Apr 18 23:40:44 2023, max compression
+gzip compressed data, was "apinator-0.0.2.tar", last modified: Wed Apr 19 19:51:20 2023, max compression
```

## Comparing `apinator-0.0.1.tar` & `apinator-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,27 @@
--rw-r--r--   0        0        0      177 2023-04-17 21:11:31.317696 apinator-0.0.1/.bumpversion.cfg
--rw-r--r--   0        0        0     2162 2022-07-05 17:25:03.902436 apinator-0.0.1/.gitignore
--rw-r--r--   0        0        0      720 2023-04-17 21:14:01.448694 apinator-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1095 2023-04-18 23:01:35.135695 apinator-0.0.1/.ruff.toml
--rw-r--r--   0        0        0        0 2023-04-17 21:12:49.553590 apinator-0.0.1/README.md
--rw-r--r--   0        0        0       94 2023-04-18 00:02:24.544849 apinator-0.0.1/apinator/__init__.py
--rw-r--r--   0        0        0     1857 2023-04-18 23:40:26.561130 apinator-0.0.1/apinator/api.py
--rw-r--r--   0        0        0     3191 2023-04-18 23:40:26.623119 apinator-0.0.1/apinator/common.py
--rw-r--r--   0        0        0     9413 2023-04-18 23:40:26.790974 apinator-0.0.1/apinator/endpoint.py
--rw-r--r--   0        0        0      526 2023-04-18 22:29:08.199553 apinator-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      696 2023-04-18 22:37:47.923942 apinator-0.0.1/setup.cfg
--rw-r--r--   0        0        0     4355 2023-04-18 23:40:26.979864 apinator-0.0.1/tests/test_basic.py
--rw-r--r--   0        0        0      485 2023-04-18 23:40:26.536764 apinator-0.0.1/tests/test_pathstr.py
--rw-r--r--   0        0        0      292 2023-04-18 23:40:26.527854 apinator-0.0.1/tests/test_request.py
--rw-r--r--   0        0        0      532 1970-01-01 00:00:00.000000 apinator-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      177 2023-04-19 19:51:13.060293 apinator-0.0.2/.bumpversion.cfg
+-rw-r--r--   0        0        0     2162 2022-07-05 17:25:03.902436 apinator-0.0.2/.gitignore
+-rw-r--r--   0        0        0      720 2023-04-17 21:14:01.448694 apinator-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1095 2023-04-18 23:01:35.135695 apinator-0.0.2/.ruff.toml
+-rw-r--r--   0        0        0    11558 2023-04-19 17:16:02.873453 apinator-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4264 2023-04-19 19:45:36.072300 apinator-0.0.2/README.md
+-rw-r--r--   0        0        0      325 2023-04-19 19:51:13.058721 apinator-0.0.2/apinator/__init__.py
+-rw-r--r--   0        0        0     1857 2023-04-18 23:40:26.561130 apinator-0.0.2/apinator/api.py
+-rw-r--r--   0        0        0     3191 2023-04-18 23:40:26.623119 apinator-0.0.2/apinator/common.py
+-rw-r--r--   0        0        0     9420 2023-04-19 18:29:57.123120 apinator-0.0.2/apinator/endpoint.py
+-rw-r--r--   0        0        0      634 2023-04-19 17:16:03.453979 apinator-0.0.2/docs/Makefile
+-rw-r--r--   0        0        0      132 2023-04-19 19:40:15.190935 apinator-0.0.2/docs/api/apinator.api.md
+-rw-r--r--   0        0        0      138 2023-04-19 19:40:15.208048 apinator-0.0.2/docs/api/apinator.common.md
+-rw-r--r--   0        0        0      142 2023-04-19 19:40:15.225072 apinator-0.0.2/docs/api/apinator.endpoint.md
+-rw-r--r--   0        0        0      244 2023-04-19 19:41:40.182895 apinator-0.0.2/docs/api/apinator.md
+-rw-r--r--   0        0        0     1247 2023-04-19 19:51:13.059773 apinator-0.0.2/docs/conf.py
+-rw-r--r--   0        0        0     6811 2023-04-19 19:44:22.793594 apinator-0.0.2/docs/getting_started.md
+-rw-r--r--   0        0        0     2809 2023-04-19 19:41:01.048308 apinator-0.0.2/docs/index.md
+-rwxr-xr-x   0        0        0      765 2023-04-19 17:16:03.486524 apinator-0.0.2/docs/make.bat
+-rw-r--r--   0        0        0     3151 2023-04-19 17:16:03.517149 apinator-0.0.2/docs/overview.md
+-rw-r--r--   0        0        0       57 2023-04-19 19:49:31.416910 apinator-0.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0      627 2023-04-19 17:16:03.446049 apinator-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      696 2023-04-19 19:51:13.058195 apinator-0.0.2/setup.cfg
+-rw-r--r--   0        0        0     4355 2023-04-18 23:40:26.979864 apinator-0.0.2/tests/test_basic.py
+-rw-r--r--   0        0        0      485 2023-04-18 23:40:26.536764 apinator-0.0.2/tests/test_pathstr.py
+-rw-r--r--   0        0        0      292 2023-04-18 23:40:26.527854 apinator-0.0.2/tests/test_request.py
+-rw-r--r--   0        0        0     5001 1970-01-01 00:00:00.000000 apinator-0.0.2/PKG-INFO
```

### Comparing `apinator-0.0.1/.gitignore` & `apinator-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `apinator-0.0.1/.pre-commit-config.yaml` & `apinator-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `apinator-0.0.1/.ruff.toml` & `apinator-0.0.2/.ruff.toml`

 * *Files identical despite different names*

### Comparing `apinator-0.0.1/apinator/api.py` & `apinator-0.0.2/apinator/api.py`

 * *Files identical despite different names*

### Comparing `apinator-0.0.1/apinator/common.py` & `apinator-0.0.2/apinator/common.py`

 * *Files identical despite different names*

### Comparing `apinator-0.0.1/apinator/endpoint.py` & `apinator-0.0.2/apinator/endpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 R = TypeVar("R", bound=BaseModel)
 M = TypeVar("M", bound=BaseModel)
 
 
 class EndpointDefinition(BaseModel, Generic[R, M]):
     name: Optional[str] = None
     url: Union[PathStr, str]
-    response_model: Optional[Type[R]]
+    response_model: Optional[Type[R]] = None
     body_model: Optional[Type[M]] = None
     method: Union[HttpMethod, str] = HttpMethod.GET
     arg_names: List[str] = ()
     default_query: Dict[str, Optional[str]] = {}
 
     class Config:
         frozen = False
```

### Comparing `apinator-0.0.1/pyproject.toml` & `apinator-0.0.2/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -16,10 +16,16 @@
 
 [project.optional-dependencies]
 tests = [
     "pytest",
     "pytest-cov",
     "responses",
 ]
+dev = [
+    "sphinx",
+    "sphinx-material",
+    "sphinxcontrib-mermaid",
+    "myst-parser",
+]
 
 [project.urls]
 Home = "https://github.com/rearc-data/apinator"
```

### Comparing `apinator-0.0.1/setup.cfg` & `apinator-0.0.2/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 7665 7273  [metadata]..vers
-00000010: 696f 6e20 3d20 302e 302e 310d 0a6e 616d  ion = 0.0.1..nam
+00000010: 696f 6e20 3d20 302e 302e 320d 0a6e 616d  ion = 0.0.2..nam
 00000020: 6520 3d20 6170 696e 6174 6f72 0d0a 6465  e = apinator..de
 00000030: 7363 7269 7074 696f 6e20 3d20 546f 6f6c  scription = Tool
 00000040: 696e 6720 746f 2062 7569 6c64 2063 6f6e  ing to build con
 00000050: 7369 7374 656e 742c 2073 656c 662d 7661  sistent, self-va
 00000060: 6c69 6461 7469 6e67 2062 696e 6469 6e67  lidating binding
 00000070: 7320 746f 2065 7874 6572 6e61 6c20 4150  s to external AP
 00000080: 4927 730d 0a61 7574 686f 7220 3d20 5265  I's..author = Re
```

### Comparing `apinator-0.0.1/tests/test_basic.py` & `apinator-0.0.2/tests/test_basic.py`

 * *Files identical despite different names*


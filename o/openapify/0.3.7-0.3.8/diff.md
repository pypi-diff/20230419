# Comparing `tmp/openapify-0.3.7.tar.gz` & `tmp/openapify-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapify-0.3.7.tar", last modified: Fri Apr 14 17:04:59 2023, max compression
+gzip compressed data, was "openapify-0.3.8.tar", last modified: Wed Apr 19 10:24:44 2023, max compression
```

## Comparing `openapify-0.3.7.tar` & `openapify-0.3.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.368747 openapify-0.3.7/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    10763 2023-04-11 22:14:24.000000 openapify-0.3.7/LICENSE
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30587 2023-04-14 17:04:59.368608 openapify-0.3.7/PKG-INFO
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    29724 2023-04-14 16:11:16.000000 openapify-0.3.7/README.md
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.365456 openapify-0.3.7/openapify/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      488 2023-04-12 20:02:29.000000 openapify-0.3.7/openapify/__init__.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.367486 openapify-0.3.7/openapify/core/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.7/openapify/core/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    15787 2023-04-14 15:56:53.000000 openapify-0.3.7/openapify/core/builder.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2120 2023-04-13 11:29:19.000000 openapify-0.3.7/openapify/core/const.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2247 2023-04-14 10:18:14.000000 openapify-0.3.7/openapify/core/document.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1720 2023-04-13 18:04:05.000000 openapify-0.3.7/openapify/core/jsonschema.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1971 2023-04-14 14:51:07.000000 openapify-0.3.7/openapify/core/models.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.367805 openapify-0.3.7/openapify/core/openapi/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.7/openapify/core/openapi/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5299 2023-04-14 15:52:57.000000 openapify-0.3.7/openapify/core/openapi/models.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5399 2023-04-14 16:53:08.000000 openapify-0.3.7/openapify/decorators.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.368048 openapify-0.3.7/openapify/ext/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.7/openapify/ext/__init__.py
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.368237 openapify-0.3.7/openapify/ext/web/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.7/openapify/ext/web/__init__.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4767 2023-04-11 22:14:24.000000 openapify-0.3.7/openapify/ext/web/aiohttp.py
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.7/openapify/py.typed
-drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-14 17:04:59.366291 openapify-0.3.7/openapify.egg-info/
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30587 2023-04-14 17:04:59.000000 openapify-0.3.7/openapify.egg-info/PKG-INFO
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      613 2023-04-14 17:04:59.000000 openapify-0.3.7/openapify.egg-info/SOURCES.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-14 17:04:59.000000 openapify-0.3.7/openapify.egg-info/dependency_links.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-10 17:48:20.000000 openapify-0.3.7/openapify.egg-info/not-zip-safe
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       42 2023-04-14 17:04:59.000000 openapify-0.3.7/openapify.egg-info/requires.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       10 2023-04-14 17:04:59.000000 openapify-0.3.7/openapify.egg-info/top_level.txt
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      364 2023-04-10 08:32:02.000000 openapify-0.3.7/pyproject.toml
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       38 2023-04-14 17:04:59.368785 openapify-0.3.7/setup.cfg
--rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1298 2023-04-14 17:03:09.000000 openapify-0.3.7/setup.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.154322 openapify-0.3.8/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    10763 2023-04-11 22:14:24.000000 openapify-0.3.8/LICENSE
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30602 2023-04-19 10:24:44.154186 openapify-0.3.8/PKG-INFO
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    29739 2023-04-19 10:07:41.000000 openapify-0.3.8/README.md
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.151073 openapify-0.3.8/openapify/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      498 2023-04-19 10:06:31.000000 openapify-0.3.8/openapify/__init__.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.153058 openapify-0.3.8/openapify/core/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.8/openapify/core/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    15792 2023-04-19 10:07:08.000000 openapify-0.3.8/openapify/core/builder.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2120 2023-04-13 11:29:19.000000 openapify-0.3.8/openapify/core/const.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     2247 2023-04-14 10:18:14.000000 openapify-0.3.8/openapify/core/document.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1720 2023-04-13 18:04:05.000000 openapify-0.3.8/openapify/core/jsonschema.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1971 2023-04-14 14:51:07.000000 openapify-0.3.8/openapify/core/models.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.153384 openapify-0.3.8/openapify/core/openapi/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.8/openapify/core/openapi/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5299 2023-04-14 15:52:57.000000 openapify-0.3.8/openapify/core/openapi/models.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     5409 2023-04-19 10:06:31.000000 openapify-0.3.8/openapify/decorators.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.153626 openapify-0.3.8/openapify/ext/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.8/openapify/ext/__init__.py
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.153814 openapify-0.3.8/openapify/ext/web/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.8/openapify/ext/web/__init__.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     4767 2023-04-11 22:14:24.000000 openapify-0.3.8/openapify/ext/web/aiohttp.py
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-10 08:32:02.000000 openapify-0.3.8/openapify/py.typed
+drwxr-xr-x   0 alexander.tikhonov   (503) staff       (20)        0 2023-04-19 10:24:44.151884 openapify-0.3.8/openapify.egg-info/
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)    30602 2023-04-19 10:24:44.000000 openapify-0.3.8/openapify.egg-info/PKG-INFO
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      613 2023-04-19 10:24:44.000000 openapify-0.3.8/openapify.egg-info/SOURCES.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-19 10:24:44.000000 openapify-0.3.8/openapify.egg-info/dependency_links.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)        1 2023-04-10 17:48:20.000000 openapify-0.3.8/openapify.egg-info/not-zip-safe
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       42 2023-04-19 10:24:44.000000 openapify-0.3.8/openapify.egg-info/requires.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       10 2023-04-19 10:24:44.000000 openapify-0.3.8/openapify.egg-info/top_level.txt
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)      364 2023-04-10 08:32:02.000000 openapify-0.3.8/pyproject.toml
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)       38 2023-04-19 10:24:44.154360 openapify-0.3.8/setup.cfg
+-rw-r--r--   0 alexander.tikhonov   (503) staff       (20)     1298 2023-04-19 10:24:17.000000 openapify-0.3.8/setup.py
```

### Comparing `openapify-0.3.7/LICENSE` & `openapify-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `openapify-0.3.7/PKG-INFO` & `openapify-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.3.7
+Version: 0.3.8
 Summary: Framework agnostic OpenAPI Specification generation for code lovers
 Home-page: https://github.com/Fatal1ty/openapify
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
@@ -278,15 +278,15 @@
     ],
     tags=["book"],
 )
 ```
 
 As will be shown further, optional
 arguments `summary`, `description`, `parameters` and `tags` can be overridden
-or extended by `path_docs` and `request_schema` decorators.
+or extended by `operation_docs` and `request_schema` decorators.
 
 The creating of these route definitions can be automated and adapted to a
 specific web-framework, and openapify has built-in support for a few of them.
 See [Integration with web-frameworks](#integration-with-web-frameworks) for
 details.
 
 Integration with web-frameworks
@@ -357,20 +357,20 @@
 the [Operation Object](https://spec.openapis.org/oas/v3.1.0#operation-object)
 which describes a single API operation on a path. We will look at what each
 decorator parameter is responsible for and how it is reflected in the final
 document.
 
 ### Generic operation info
 
-Decorator `path_docs` adds generic information about the Operation object,
+Decorator `operation_docs` adds generic information about the Operation object,
 which includes summary, description, tags, external documentation and
 deprecation marker.
 
 ```python
-from openapify import path_docs
+from openapify import operation_docs
 ```
 
 #### summary
 
 An optional, string summary, intended to apply to the operation. This affects
 the value of
 the [`summary`](https://spec.openapis.org/oas/v3.1.0#operation-object) field of
```

### Comparing `openapify-0.3.7/README.md` & `openapify-0.3.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
     ],
     tags=["book"],
 )
 ```
 
 As will be shown further, optional
 arguments `summary`, `description`, `parameters` and `tags` can be overridden
-or extended by `path_docs` and `request_schema` decorators.
+or extended by `operation_docs` and `request_schema` decorators.
 
 The creating of these route definitions can be automated and adapted to a
 specific web-framework, and openapify has built-in support for a few of them.
 See [Integration with web-frameworks](#integration-with-web-frameworks) for
 details.
 
 Integration with web-frameworks
@@ -334,20 +334,20 @@
 the [Operation Object](https://spec.openapis.org/oas/v3.1.0#operation-object)
 which describes a single API operation on a path. We will look at what each
 decorator parameter is responsible for and how it is reflected in the final
 document.
 
 ### Generic operation info
 
-Decorator `path_docs` adds generic information about the Operation object,
+Decorator `operation_docs` adds generic information about the Operation object,
 which includes summary, description, tags, external documentation and
 deprecation marker.
 
 ```python
-from openapify import path_docs
+from openapify import operation_docs
 ```
 
 #### summary
 
 An optional, string summary, intended to apply to the operation. This affects
 the value of
 the [`summary`](https://spec.openapis.org/oas/v3.1.0#operation-object) field of
```

### Comparing `openapify-0.3.7/openapify/core/builder.py` & `openapify-0.3.8/openapify/core/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                     parameters.extend(self._build_request_headers(headers))
                 cookies = args.get("cookies")
                 if cookies:
                     parameters.extend(self._build_cookies(cookies))
 
             elif args_type == "response":
                 responses = self._update_responses(responses=responses, **args)
-            elif args_type == "path_docs":
+            elif args_type == "operation_docs":
                 args = args.copy()
                 summary = args.get("summary")
                 description = args.get("description")
                 tags.extend(args.get("tags") or [])
                 # _merge_parameters(parameters, args.get("parameters") or {})
                 operation_id = args.get("operation_id")
                 external_docs = self._build_external_docs(
```

### Comparing `openapify-0.3.7/openapify/core/const.py` & `openapify-0.3.8/openapify/core/const.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.7/openapify/core/document.py` & `openapify-0.3.8/openapify/core/document.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.7/openapify/core/jsonschema.py` & `openapify-0.3.8/openapify/core/jsonschema.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.7/openapify/core/models.py` & `openapify-0.3.8/openapify/core/models.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.7/openapify/core/openapi/models.py` & `openapify-0.3.8/openapify/core/openapi/models.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.7/openapify/decorators.py` & `openapify-0.3.8/openapify/decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,30 +127,30 @@
             ),
         )
         return handler
 
     return decorator
 
 
-def path_docs(
+def operation_docs(
     summary: Optional[str] = None,
     description: Optional[str] = None,
     tags: Optional[Sequence[str]] = None,
     # parameters: Optional[Mapping[str, Union[str, Parameter]]] = None,
     operation_id: Optional[str] = None,
     external_docs: Optional[Union[str, Tuple[str, str]]] = None,
     deprecated: Optional[bool] = None,
 ) -> Callable[[Handler], Handler]:
     def decorator(handler: Handler) -> Handler:
         meta = getattr(handler, __openapify__, [])
         if not meta:
             handler.__openapify__ = meta  # type: ignore[attr-defined]
         meta.append(
             (
-                "path_docs",
+                "operation_docs",
                 {
                     "summary": summary,
                     "description": description,
                     "tags": tags,
                     # "parameters": parameters,
                     "operation_id": operation_id,
                     "external_docs": external_docs,
```

### Comparing `openapify-0.3.7/openapify/ext/web/aiohttp.py` & `openapify-0.3.8/openapify/ext/web/aiohttp.py`

 * *Files identical despite different names*

### Comparing `openapify-0.3.7/openapify.egg-info/PKG-INFO` & `openapify-0.3.8/openapify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapify
-Version: 0.3.7
+Version: 0.3.8
 Summary: Framework agnostic OpenAPI Specification generation for code lovers
 Home-page: https://github.com/Fatal1ty/openapify
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
@@ -278,15 +278,15 @@
     ],
     tags=["book"],
 )
 ```
 
 As will be shown further, optional
 arguments `summary`, `description`, `parameters` and `tags` can be overridden
-or extended by `path_docs` and `request_schema` decorators.
+or extended by `operation_docs` and `request_schema` decorators.
 
 The creating of these route definitions can be automated and adapted to a
 specific web-framework, and openapify has built-in support for a few of them.
 See [Integration with web-frameworks](#integration-with-web-frameworks) for
 details.
 
 Integration with web-frameworks
@@ -357,20 +357,20 @@
 the [Operation Object](https://spec.openapis.org/oas/v3.1.0#operation-object)
 which describes a single API operation on a path. We will look at what each
 decorator parameter is responsible for and how it is reflected in the final
 document.
 
 ### Generic operation info
 
-Decorator `path_docs` adds generic information about the Operation object,
+Decorator `operation_docs` adds generic information about the Operation object,
 which includes summary, description, tags, external documentation and
 deprecation marker.
 
 ```python
-from openapify import path_docs
+from openapify import operation_docs
 ```
 
 #### summary
 
 An optional, string summary, intended to apply to the operation. This affects
 the value of
 the [`summary`](https://spec.openapis.org/oas/v3.1.0#operation-object) field of
```

### Comparing `openapify-0.3.7/openapify.egg-info/SOURCES.txt` & `openapify-0.3.8/openapify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openapify-0.3.7/setup.py` & `openapify-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="openapify",
-    version="0.3.7",
+    version="0.3.8",
     description=(
         "Framework agnostic OpenAPI Specification generation for code lovers"
     ),
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     platforms="all",
     classifiers=[
```


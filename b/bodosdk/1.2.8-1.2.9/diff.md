# Comparing `tmp/bodosdk-1.2.8.tar.gz` & `tmp/bodosdk-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bodosdk-1.2.8.tar", last modified: Tue Mar 28 22:42:21 2023, max compression
+gzip compressed data, was "bodosdk-1.2.9.tar", last modified: Wed Apr 19 11:27:10 2023, max compression
```

## Comparing `bodosdk-1.2.8.tar` & `bodosdk-1.2.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 22:42:21.127705 bodosdk-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-03-28 22:42:16.000000 bodosdk-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-03-28 22:42:16.000000 bodosdk-1.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    34901 2023-03-28 22:42:21.127705 bodosdk-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    34206 2023-03-28 22:42:16.000000 bodosdk-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 22:42:21.131705 bodosdk-1.2.8/bodosdk/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2023-03-28 22:42:21.131705 bodosdk-1.2.8/bodosdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 22:42:21.127705 bodosdk-1.2.8/bodosdk/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (122)      774 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/api/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/api/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     7389 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/api/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/api/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    11340 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/api/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/api/request_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/api/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/api/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 22:42:21.127705 bodosdk-1.2.8/bodosdk/client/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/client/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/client/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/client/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     5931 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/client/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/client/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)     4228 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/client/job.py
--rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/client/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/client/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/client/workspace.py
--rw-r--r--   0 runner    (1001) docker     (122)      308 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/exc.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 22:42:21.127705 bodosdk-1.2.8/bodosdk/models/
--rw-r--r--   0 runner    (1001) docker     (122)     1142 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2465 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/models/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/models/catalog.py
--rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/models/cloud_config.py
--rw-r--r--   0 runner    (1001) docker     (122)     3198 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/models/cluster.py
--rw-r--r--   0 runner    (1001) docker     (122)      416 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/models/instance_role.py
--rw-r--r--   0 runner    (1001) docker     (122)    11635 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/models/job.py
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/models/secret_group.py
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/models/secrets.py
--rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-03-28 22:42:16.000000 bodosdk-1.2.8/bodosdk/models/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-28 22:42:21.127705 bodosdk-1.2.8/bodosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    34901 2023-03-28 22:42:21.000000 bodosdk-1.2.8/bodosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-03-28 22:42:21.000000 bodosdk-1.2.8/bodosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-28 22:42:21.000000 bodosdk-1.2.8/bodosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-03-28 22:42:21.000000 bodosdk-1.2.8/bodosdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-03-28 22:42:21.000000 bodosdk-1.2.8/bodosdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-03-28 22:42:21.127705 bodosdk-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-03-28 22:42:16.000000 bodosdk-1.2.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    80044 2023-03-28 22:42:16.000000 bodosdk-1.2.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:10.780630 bodosdk-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-19 11:27:05.000000 bodosdk-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-04-19 11:27:05.000000 bodosdk-1.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    34901 2023-04-19 11:27:10.780630 bodosdk-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    34206 2023-04-19 11:27:05.000000 bodosdk-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:10.780630 bodosdk-1.2.9/bodosdk/
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-04-19 11:27:10.780630 bodosdk-1.2.9/bodosdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:10.776630 bodosdk-1.2.9/bodosdk/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1591 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3313 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7389 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2867 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11856 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/request_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2963 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3982 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:10.780630 bodosdk-1.2.9/bodosdk/client/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5396 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2147 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2278 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5931 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8896 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1462 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1916 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/client/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (122)      308 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/exc.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:10.780630 bodosdk-1.2.9/bodosdk/models/
+-rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3670 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/cloud_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3198 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (122)      416 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/instance_role.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12486 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/job.py
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/secret_group.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3333 2023-04-19 11:27:05.000000 bodosdk-1.2.9/bodosdk/models/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 11:27:10.776630 bodosdk-1.2.9/bodosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    34901 2023-04-19 11:27:10.000000 bodosdk-1.2.9/bodosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-04-19 11:27:10.000000 bodosdk-1.2.9/bodosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 11:27:10.000000 bodosdk-1.2.9/bodosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-19 11:27:10.000000 bodosdk-1.2.9/bodosdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-04-19 11:27:10.000000 bodosdk-1.2.9/bodosdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-04-19 11:27:10.780630 bodosdk-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1115 2023-04-19 11:27:05.000000 bodosdk-1.2.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    80044 2023-04-19 11:27:05.000000 bodosdk-1.2.9/versioneer.py
```

### Comparing `bodosdk-1.2.8/LICENSE` & `bodosdk-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/PKG-INFO` & `bodosdk-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 1.2.8
+Version: 1.2.9
 Summary: Bodo Platform SDK
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodosdk-1.2.8/README.md` & `bodosdk-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/api/auth.py` & `bodosdk-1.2.9/bodosdk/api/auth.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/api/base.py` & `bodosdk-1.2.9/bodosdk/api/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/api/catalog.py` & `bodosdk-1.2.9/bodosdk/api/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/api/cloud_config.py` & `bodosdk-1.2.9/bodosdk/api/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/api/cluster.py` & `bodosdk-1.2.9/bodosdk/api/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/api/instance_role.py` & `bodosdk-1.2.9/bodosdk/api/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/api/job.py` & `bodosdk-1.2.9/bodosdk/api/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import List
+from datetime import datetime
+from typing import List, Union
 from uuid import UUID
 
 from pydantic import validate_arguments
 
 from bodosdk.api.base import BackendApi
 from bodosdk.exc import (
     ResourceNotFound,
@@ -17,26 +18,37 @@
     JobCreateResponse,
     CreateBatchJobDefinition,
     BatchJobDefinitionResponse,
     JobConfigOverride,
     JobRunResponse,
     PaginationDetails,
     JobRunType,
+    CreateJobRun,
+    JobRunStatus,
 )
 
 
 # helper function to compose query string from query parameters
 def build_query_string(args):
     if len(args) == 0:
         return ""
     query_string = "?"
+    counter = 0
     for k, v in args.items():
         if v is not None:
-            query_string += f"{k}={v}&"
-
+            if isinstance(v, list):
+                query_string += f"{k}="
+                for item in v[:-2]:
+                    query_string += {item} + ","
+                query_string += f"{v[-1]}&"
+            else:
+                query_string += f"{k}={v}&"
+            counter += 1
+    if counter == 0:
+        return ""
     return query_string
 
 
 class JobApi(BackendApi):
     def __init__(self, *args, **kwargs):
         super(JobApi, self).__init__(*args, **kwargs)
         self._resource_url = "job"
@@ -169,37 +181,42 @@
     # Todo: add query semantics for filtering
     @validate_arguments
     def list_batch_job_definitions(
         self,
         pagination_details: PaginationDetails = None,
     ) -> List[BatchJobDefinitionResponse]:
         args = locals()
-        args.pop("self")
+        args_keys = list(args.keys())
+        args_keys.remove("self")
+        query_string_args = dict([(key, args[key]) for key in args_keys])
         headers = self.get_auth_header()
         resource_url = (
             f"{self.get_resource_url()}/batch_job_def{build_query_string(args)}"
         )
         resp = self._requests.get(resource_url, headers=headers)
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable
+        if self(resp.status_code).startswith("4"):
+            raise ResourceNotFound(resp.json()["message"])
+
         result = []
         for json_data in resp.json():
             result.append(BatchJobDefinitionResponse(**json_data))
         return result
 
     @validate_arguments
     def get_batch_job_definition(self, uuid: UUID) -> BatchJobDefinitionResponse:
         headers = self.get_auth_header()
         resp = self._requests.get(
             f"{self.get_resource_url()}/batch_job_def/{uuid}", headers=headers
         )
         if resp.status_code == 404:
             raise ResourceNotFound
         if str(resp.status_code).startswith("5"):
-            raise ServiceUnavailable
+            raise ServiceUnavailable(resp.content)
         json_data = resp.json()
         return BatchJobDefinitionResponse(**json_data)
 
     @validate_arguments
     def update_batch_job_definition(
         self, uuid: UUID, config_override: JobConfigOverride
     ) -> BatchJobDefinitionResponse:
@@ -220,25 +237,24 @@
             )
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable
         raise UnknownError(resp.content)
 
     # Job Run APIs
     @validate_arguments
-    def create_batch_job_run(self, job_definition: JobDefinition) -> JobRunResponse:
+    def create_batch_job_run(self, create_job_run: CreateJobRun) -> JobRunResponse:
         headers = {"Content-type": "application/json"}
         headers.update(self.get_auth_header())
         resp = self._requests.post(
             f"{self.get_resource_url()}/run/batch",
-            data=job_definition.json(by_alias=True),
+            data=create_job_run.json(by_alias=True),
             headers=headers,
         )
         if str(resp.status_code).startswith("2"):
             return JobRunResponse(**resp.json())
-            # TODO (Ritwika) : confirm action for environment variables etc.
         if resp.status_code == 404:
             raise ResourceNotFound("Batch job definition not found")
         if resp.status_code == 409:
             raise ResourceNotFound(
                 "May have specified a default cluster which doesn't belong the workspace"
             )
         if str(resp.status_code).startswith("5"):
@@ -270,40 +286,32 @@
         if str(resp.status_code).startswith("5"):
             raise ServiceUnavailable
         return
 
     @validate_arguments
     def list_job_runs(
         self,
-        job_type: JobRunType = None,
-        batch_job_id=None,
-        status=None,
-        cluster_id=None,
-        started_at=None,
-        finished_at=None,
+        job_type: List[JobRunType] = None,
+        batch_job_id: Union[List[UUID], None] = None,
+        status: Union[List[JobRunStatus], None] = None,
+        cluster_id: Union[List[UUID], None] = None,
+        started_at: Union[datetime, None] = None,
+        finished_at: Union[datetime, None] = None,
         pagination_details=None,
     ) -> List[JobRunResponse]:
         args = locals()
-        args.pop("self")
-        args.pop("job_type")
-        query_string_args = dict(
-            (key, args[key]) for key in list(args.keys()) if args[key]
-        )
+        args_keys = list(args.keys())
+        args_keys.remove("self")
+        query_string_args = dict([(key, args[key]) for key in args_keys])
         headers = self.get_auth_header()
-        job_type_url_suffix = None
-        if job_type:
-            job_type_url_suffix = job_type.lower()
-        headers = self.get_auth_header()
-        if job_type_url_suffix:
-            resp = self._requests.get(
-                f"{self.get_resource_url()}/run/{job_type_url_suffix}{build_query_string(query_string_args)}",
-                headers=headers,
-            )
-        else:
-            resp = self._requests.get(f"{self.get_resource_url()}/run", headers=headers)
-
+        headers = self.get_auth_header()
+        query_string = build_query_string(query_string_args)
+        url = f"{self.get_resource_url()}/run{query_string}"
+        resp = self._requests.get(url, headers=headers)
         if str(resp.status_code).startswith("5"):
-            raise ServiceUnavailable
+            raise ServiceUnavailable()
+        if str(resp.status_code).startswith("4"):
+            raise ResourceNotFound(resp.json()["message"])
         result = []
         for json_data in resp.json():
             result.append(JobRunResponse(**json_data))
         return result
```

### Comparing `bodosdk-1.2.8/bodosdk/api/request_wrapper.py` & `bodosdk-1.2.9/bodosdk/api/request_wrapper.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/api/secret_group.py` & `bodosdk-1.2.9/bodosdk/api/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/api/secrets.py` & `bodosdk-1.2.9/bodosdk/api/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/api/workspace.py` & `bodosdk-1.2.9/bodosdk/api/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/client/base.py` & `bodosdk-1.2.9/bodosdk/client/base.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/client/catalog.py` & `bodosdk-1.2.9/bodosdk/client/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/client/cloud_config.py` & `bodosdk-1.2.9/bodosdk/client/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/client/cluster.py` & `bodosdk-1.2.9/bodosdk/client/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/client/instance_role.py` & `bodosdk-1.2.9/bodosdk/client/instance_role.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/client/secret_group.py` & `bodosdk-1.2.9/bodosdk/client/secret_group.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/client/secrets.py` & `bodosdk-1.2.9/bodosdk/client/secrets.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/client/workspace.py` & `bodosdk-1.2.9/bodosdk/client/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/models/__init__.py` & `bodosdk-1.2.9/bodosdk/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -51,8 +51,17 @@
     JobDefinition,
     JobSourceType,
     GitRepoSource,
     S3Source,
     WorkspaceSource,
     JobCluster,
     JobExecution,
+    BatchJobDefinitionResponse,
+    CreateBatchJobDefinition,
+    JobConfig,
+    JobConfigOverride,
+    WorkspaceDef,
+    SourceCodeType,
+    RetryStrategy,
+    JobSource,
+    JobSourceType,
 )
```

### Comparing `bodosdk-1.2.8/bodosdk/models/base.py` & `bodosdk-1.2.9/bodosdk/models/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,14 +59,15 @@
     PAUSING - when operation of stopping machines is in progress
     RESUMING - when operation of starting machines is in progress
     """
 
     NEW = "NEW"
     INPROGRESS = "INPROGRESS"
     ASGCREATED = "ASGCREATED"
+    INITIALIZING = "INITIALIZING"
     SCALING = "SCALING"
     RUNNING = "RUNNING"
     FAILED = "FAILED"
     TERMINATING = "TERMINATING"
     TERMINATED = "TERMINATED"
     PAUSED = "PAUSED"
     PAUSING = "PAUSING"
```

### Comparing `bodosdk-1.2.8/bodosdk/models/catalog.py` & `bodosdk-1.2.9/bodosdk/models/catalog.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/models/cloud_config.py` & `bodosdk-1.2.9/bodosdk/models/cloud_config.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/models/cluster.py` & `bodosdk-1.2.9/bodosdk/models/cluster.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk/models/job.py` & `bodosdk-1.2.9/bodosdk/models/job.py`

 * *Files 18% similar despite different names*

```diff
@@ -259,18 +259,18 @@
         Job environment variables. (Default: {})
 
     """
 
     source: JobSource
     source_code_type: SourceCodeType = Field(..., alias="type")
     sourceLocation: str
-    args: Union[str, Dict] = Field(default_factory=dict)
+    args: Union[str, Dict, None] = Field(default_factory=dict)
     retry_strategy: RetryStrategy = Field(RetryStrategy(), alias="retryStrategy")
     timeout: int = 60
-    env_vars: Dict = Field(default_factory=dict, alias="envVars")
+    env_vars: Union[None, Dict] = Field(default_factory=dict, alias="envVars")
 
 
 class JobConfigOverride(CamelCaseBase):
     """
     Job configuration override.
 
     ...
@@ -339,15 +339,15 @@
 
 
 class JobRunType(str, enum.Enum):
     BATCH = "BATCH"
     INTERACTIVE = "INTERACTIVE"
 
 
-class JobRunStatus(enum.Enum):
+class JobRunStatus(str, enum.Enum):
     PENDING = "PENDING"
     RUNNING = "RUNNING"
     SUCCEEDED = "SUCCEEDED"
     FAILED = "FAILED"
     CANCELLED = "CANCELLED"
     CANCELLING = "CANCELLING"
 
@@ -399,25 +399,31 @@
     lastKnownActivity: Optional[datetime]
         Job run last known activity.
 
     """
 
     uuid: UUID
     name: str
-    clusterUUID: UUID = Field(..., alias="clusterUUID")
+    clusterUUID: Optional[Union[UUID, None]] = Field(default=None, alias="clusterUUID")
     type: JobRunType
     config: JobConfig
     submittedAt: datetime = Field(..., alias="submittedAt")
-    finishedAt: datetime = Field(..., alias="finishedAt")
-    startedAt: datetime = Field(..., alias="startedAt")
+    finishedAt: Optional[Union[datetime, None]] = Field(
+        default=None, alias="finishedAt"
+    )
+    startedAt: Optional[Union[datetime, None]] = Field(default=None, alias="startedAt")
     status: JobRunStatus
     batchJobDefinitionConfigOverrides: Optional[JobConfigOverride]
     numRetriesUsed: int = Field(..., alias="numRetriesUsed")
-    lastHealthCheck: Optional[datetime] = Field(..., alias="lastHealthCheck")
-    lastKnownActivity: Optional[datetime] = Field(..., alias="lastknownActivity")
+    lastHealthCheck: Optional[Union[datetime, None]] = Field(
+        default=None, alias="lastHealthCheck"
+    )
+    lastKnownActivity: Optional[Union[datetime, None]] = Field(
+        default=None, alias="lastknownActivity"
+    )
 
 
 class BatchJobDefinitionResponse(CamelCaseBase):
     """
     Batch job definition response.
 
     ...
@@ -455,14 +461,41 @@
     clusterUUID: Optional[str]  # Todo(Ritwika): Confirm
     created_by: str = Field(..., alias="createdBy")
     job_runs: List[JobRunResponse] = Field(default_factory=list, alias="jobRuns")
     # Run related fields
     # Rules related fields
 
 
+class CreateJobRun(CamelCaseBase):
+    """
+    Create job run.
+
+    ...
+
+    Attributes
+    ----------
+    type: JobRunType
+        Job run type.
+
+    clusterUUID: Optional[str]
+        Job cluster UUID.
+
+    batchJobUUID: Optional[str]
+        Batch job UUID.
+
+    batchJobDefinitionConfigOverrides: Optional[JobConfigOverride]
+        Batch job definition configuration overrides.
+    """
+
+    type: JobRunType = JobRunType.BATCH
+    clusterUUID: Optional[str]  # Todo(Ritwika): Confirm
+    batchJobDefinitionUUID: Optional[str] = Field(..., alias="batchJobDefinitionUUID")
+    batchJobDefinitionConfigOverrides: Optional[JobConfigOverride]
+
+
 class PaginationOrder(str, enum.Enum):
     ASC = "ASC"
     DESC = "DESC"
 
 
 class PaginationDetails(CamelCaseBase):
     """
```

### Comparing `bodosdk-1.2.8/bodosdk/models/workspace.py` & `bodosdk-1.2.9/bodosdk/models/workspace.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/bodosdk.egg-info/PKG-INFO` & `bodosdk-1.2.9/bodosdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bodosdk
-Version: 1.2.8
+Version: 1.2.9
 Summary: Bodo Platform SDK
 Home-page: https://github.com/Bodo-inc/bodo-sdk
 Author: Bodo, Inc.
 Author-email: noreply@bodo.ai
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bodosdk-1.2.8/bodosdk.egg-info/SOURCES.txt` & `bodosdk-1.2.9/bodosdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/setup.py` & `bodosdk-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `bodosdk-1.2.8/versioneer.py` & `bodosdk-1.2.9/versioneer.py`

 * *Files identical despite different names*


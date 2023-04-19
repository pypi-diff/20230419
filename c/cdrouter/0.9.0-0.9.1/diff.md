# Comparing `tmp/cdrouter-0.9.0.tar.gz` & `tmp/cdrouter-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cdrouter-0.9.0.tar", last modified: Thu Mar 30 14:08:55 2023, max compression
+gzip compressed data, was "dist/cdrouter-0.9.1.tar", last modified: Wed Apr 19 17:46:31 2023, max compression
```

## Comparing `cdrouter-0.9.0.tar` & `cdrouter-0.9.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:08:55.000000 cdrouter-0.9.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:08:55.000000 cdrouter-0.9.0/cdrouter/
--rw-r--r--   0 root         (0) root         (0)      162 2023-03-30 14:08:55.000000 cdrouter-0.9.0/cdrouter/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13094 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/alerts.py
--rw-r--r--   0 root         (0) root         (0)     4695 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/annotations.py
--rw-r--r--   0 root         (0) root         (0)     7278 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/attachments.py
--rw-r--r--   0 root         (0) root         (0)     4691 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/captures.py
--rw-r--r--   0 root         (0) root         (0)     1393 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/cdr_datetime.py
--rw-r--r--   0 root         (0) root         (0)      246 2020-11-05 19:50:12.000000 cdrouter-0.9.0/cdrouter/cdr_error.py
--rw-r--r--   0 root         (0) root         (0)    18207 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/cdrouter.py
--rw-r--r--   0 root         (0) root         (0)    19895 2023-03-30 14:07:53.000000 cdrouter-0.9.0/cdrouter/configs.py
--rw-r--r--   0 root         (0) root         (0)    16563 2023-03-30 14:07:53.000000 cdrouter-0.9.0/cdrouter/devices.py
--rw-r--r--   0 root         (0) root         (0)     1755 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/exports.py
--rw-r--r--   0 root         (0) root         (0)     7027 2023-02-02 15:33:12.000000 cdrouter-0.9.0/cdrouter/filters.py
--rw-r--r--   0 root         (0) root         (0)     4588 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/highlights.py
--rw-r--r--   0 root         (0) root         (0)     3429 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/history.py
--rw-r--r--   0 root         (0) root         (0)     9360 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/imports.py
--rw-r--r--   0 root         (0) root         (0)    11003 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/jobs.py
--rw-r--r--   0 root         (0) root         (0)    10408 2023-03-30 14:08:03.000000 cdrouter-0.9.0/cdrouter/metrics.py
--rw-r--r--   0 root         (0) root         (0)    15834 2023-03-30 14:07:53.000000 cdrouter-0.9.0/cdrouter/packages.py
--rw-r--r--   0 root         (0) root         (0)    37936 2023-03-30 14:08:03.000000 cdrouter-0.9.0/cdrouter/results.py
--rw-r--r--   0 root         (0) root         (0)    20907 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/system.py
--rw-r--r--   0 root         (0) root         (0)     4425 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/tags.py
--rw-r--r--   0 root         (0) root         (0)    20060 2023-03-30 14:08:03.000000 cdrouter-0.9.0/cdrouter/testresults.py
--rw-r--r--   0 root         (0) root         (0)    23930 2022-11-02 12:33:34.000000 cdrouter-0.9.0/cdrouter/testsuites.py
--rw-r--r--   0 root         (0) root         (0)     8849 2023-03-30 14:07:53.000000 cdrouter-0.9.0/cdrouter/users.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-30 14:08:55.000000 cdrouter-0.9.0/cdrouter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7138 2023-03-30 14:08:55.000000 cdrouter-0.9.0/cdrouter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      728 2023-03-30 14:08:55.000000 cdrouter-0.9.0/cdrouter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-30 14:08:55.000000 cdrouter-0.9.0/cdrouter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2023-03-30 14:08:55.000000 cdrouter-0.9.0/cdrouter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-30 14:08:55.000000 cdrouter-0.9.0/cdrouter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1073 2020-11-05 19:50:12.000000 cdrouter-0.9.0/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       64 2020-11-05 19:50:12.000000 cdrouter-0.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4981 2023-03-01 14:31:24.000000 cdrouter-0.9.0/README.rst
--rw-r--r--   0 root         (0) root         (0)       61 2022-11-02 12:33:34.000000 cdrouter-0.9.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       67 2023-03-30 14:08:55.000000 cdrouter-0.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2022 2022-11-02 12:33:34.000000 cdrouter-0.9.0/setup.py
--rw-r--r--   0 root         (0) root         (0)     7138 2023-03-30 14:08:55.000000 cdrouter-0.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:46:31.000000 cdrouter-0.9.1/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter/
+-rw-r--r--   0 root         (0) root         (0)      162 2023-04-19 17:46:30.000000 cdrouter-0.9.1/cdrouter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13094 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/alerts.py
+-rw-r--r--   0 root         (0) root         (0)     4695 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/annotations.py
+-rw-r--r--   0 root         (0) root         (0)     7278 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/attachments.py
+-rw-r--r--   0 root         (0) root         (0)     4691 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/captures.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2022-11-02 12:33:34.000000 cdrouter-0.9.1/cdrouter/cdr_datetime.py
+-rw-r--r--   0 root         (0) root         (0)      246 2020-11-05 19:50:12.000000 cdrouter-0.9.1/cdrouter/cdr_error.py
+-rw-r--r--   0 root         (0) root         (0)    18267 2023-04-19 17:46:00.000000 cdrouter-0.9.1/cdrouter/cdrouter.py
+-rw-r--r--   0 root         (0) root         (0)    19895 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/configs.py
+-rw-r--r--   0 root         (0) root         (0)    16563 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/devices.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2022-11-02 12:33:34.000000 cdrouter-0.9.1/cdrouter/exports.py
+-rw-r--r--   0 root         (0) root         (0)     7027 2023-02-02 15:33:12.000000 cdrouter-0.9.1/cdrouter/filters.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/highlights.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/history.py
+-rw-r--r--   0 root         (0) root         (0)     9360 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/imports.py
+-rw-r--r--   0 root         (0) root         (0)    11003 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/jobs.py
+-rw-r--r--   0 root         (0) root         (0)    10408 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/metrics.py
+-rw-r--r--   0 root         (0) root         (0)    15834 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/packages.py
+-rw-r--r--   0 root         (0) root         (0)    37996 2023-04-19 17:46:00.000000 cdrouter-0.9.1/cdrouter/results.py
+-rw-r--r--   0 root         (0) root         (0)    20907 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/system.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/tags.py
+-rw-r--r--   0 root         (0) root         (0)    20060 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/testresults.py
+-rw-r--r--   0 root         (0) root         (0)    23930 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/testsuites.py
+-rw-r--r--   0 root         (0) root         (0)     8849 2023-04-19 15:35:17.000000 cdrouter-0.9.1/cdrouter/users.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      728 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-04-19 17:46:31.000000 cdrouter-0.9.1/cdrouter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1073 2020-11-05 19:50:12.000000 cdrouter-0.9.1/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2020-11-05 19:50:12.000000 cdrouter-0.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4981 2023-03-01 14:31:24.000000 cdrouter-0.9.1/README.rst
+-rw-r--r--   0 root         (0) root         (0)       61 2022-11-02 12:33:34.000000 cdrouter-0.9.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2023-04-19 17:46:31.000000 cdrouter-0.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2022 2022-11-02 12:33:34.000000 cdrouter-0.9.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)     7138 2023-04-19 17:46:31.000000 cdrouter-0.9.1/PKG-INFO
```

### Comparing `cdrouter-0.9.0/cdrouter/alerts.py` & `cdrouter-0.9.1/cdrouter/alerts.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/annotations.py` & `cdrouter-0.9.1/cdrouter/annotations.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/attachments.py` & `cdrouter-0.9.1/cdrouter/attachments.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/captures.py` & `cdrouter-0.9.1/cdrouter/captures.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/cdr_datetime.py` & `cdrouter-0.9.1/cdrouter/cdr_datetime.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/cdrouter.py` & `cdrouter-0.9.1/cdrouter/cdrouter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
-# Copyright (c) 2017-2022 by QA Cafe.
+# Copyright (c) 2017-2023 by QA Cafe.
 # All Rights Reserved.
 #
 
 from builtins import input
 import getpass
 import io
 import os
@@ -11,15 +11,15 @@
 from threading import Lock
 import requests
 from requests_toolbelt.downloadutils import stream
 from requests_toolbelt import sessions
 from requests_toolbelt.utils.user_agent import user_agent
 from requests.packages.urllib3.exceptions import InsecureRequestWarning # pylint: disable=import-error
 from requests.exceptions import HTTPError
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 
 from . import __version__
 from .cdr_error import CDRouterError
 from .cdr_datetime import DateTime
 from .alerts import AlertsService
 from .configs import ConfigsService
 from .devices import DevicesService
@@ -382,15 +382,15 @@
                 resp.raise_for_status()
             except HTTPError as he:
                 message = str(he)
 
             try:
                 json = resp.json()
                 resp_schema = ResponseSchema()
-                result = resp_schema.load(json)
+                result = resp_schema.load(json, unknown=EXCLUDE)
                 if result.error is not None:
                     message = result.error
             except HTTPError as he:
                 message = str(he)
             except: # pylint: disable=bare-except
                 pass
 
@@ -398,20 +398,20 @@
 
     def decode(self, schema, resp, many=None, links=False):
         json = resp.json()
         resp_schema = ResponseSchema()
         if many is True:
             resp_schema = ListResponseSchema()
 
-        result = resp_schema.load(json)
+        result = resp_schema.load(json, unknown=EXCLUDE)
 
         if result.data is None:
             raise CDRouterError('no data field in JSON response!', response=resp)
 
-        data = schema.load(result.data, many=many)
+        data = schema.load(result.data, unknown=EXCLUDE, many=many)
 
         if many is True and links is True and result.links is not None:
             return (data, result.links)
 
         return data
 
     def encode(self, schema, resource, many=None, skip_none=False):
```

### Comparing `cdrouter-0.9.0/cdrouter/configs.py` & `cdrouter-0.9.1/cdrouter/configs.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/devices.py` & `cdrouter-0.9.1/cdrouter/devices.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/exports.py` & `cdrouter-0.9.1/cdrouter/exports.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/filters.py` & `cdrouter-0.9.1/cdrouter/filters.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/highlights.py` & `cdrouter-0.9.1/cdrouter/highlights.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/history.py` & `cdrouter-0.9.1/cdrouter/history.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/imports.py` & `cdrouter-0.9.1/cdrouter/imports.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/jobs.py` & `cdrouter-0.9.1/cdrouter/jobs.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/metrics.py` & `cdrouter-0.9.1/cdrouter/metrics.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/packages.py` & `cdrouter-0.9.1/cdrouter/packages.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/results.py` & `cdrouter-0.9.1/cdrouter/results.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 """Module for accessing CDRouter Results."""
 
 from collections import namedtuple
 import io
 
 from requests_toolbelt.downloadutils import stream
-from marshmallow import Schema, fields, post_load
+from marshmallow import Schema, fields, post_load, EXCLUDE
 from .cdr_datetime import DateTime
 from .testresults import TestResultSchema
 from .alerts import AlertSchema
 from .configs import InterfacesSchema
 from .metrics import GraphMetric, GraphMetricSchema, Page as MetricPage, MetricSchema as MetricsDotMetricSchema
 
 class TestCount(object):
@@ -400,19 +400,19 @@
     @post_load
     def post_load(self, data, **kwargs): # pylint: disable=unused-argument
         return Feature(**data)
 
 class UpdateField(fields.Field):
     def _deserialize(self, value, attr, data, **kwargs):
         if 'result' in value and 'status' in value:
-            return ResultSchema().load(value)
+            return ResultSchema().load(value, unknown=EXCLUDE)
         if 'result' in value and 'status' not in value:
-            return TestResultSchema().load(value)
+            return TestResultSchema().load(value, unknown=EXCLUDE)
         if 'sid' in value and 'rev' in value:
-            return AlertSchema().load(value)
+            return AlertSchema().load(value, unknown=EXCLUDE)
         self.fail('invalid')
         return None
 
 class Update(object):
     """Model for CDRouter Result Update.
 
     :param id: (optional) Update ID as an int.
```

### Comparing `cdrouter-0.9.0/cdrouter/system.py` & `cdrouter-0.9.1/cdrouter/system.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/tags.py` & `cdrouter-0.9.1/cdrouter/tags.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/testresults.py` & `cdrouter-0.9.1/cdrouter/testresults.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/testsuites.py` & `cdrouter-0.9.1/cdrouter/testsuites.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter/users.py` & `cdrouter-0.9.1/cdrouter/users.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/cdrouter.egg-info/PKG-INFO` & `cdrouter-0.9.1/cdrouter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cdrouter
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python client for the CDRouter Web API
 Home-page: https://github.com/qacafe/cdrouter.py
 Author: QA Cafe
 Author-email: support@qacafe.com
 License: MIT
 Description: cdrouter
         ========
```

### Comparing `cdrouter-0.9.0/cdrouter.egg-info/SOURCES.txt` & `cdrouter-0.9.1/cdrouter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/LICENSE.txt` & `cdrouter-0.9.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/README.rst` & `cdrouter-0.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/setup.py` & `cdrouter-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `cdrouter-0.9.0/PKG-INFO` & `cdrouter-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cdrouter
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python client for the CDRouter Web API
 Home-page: https://github.com/qacafe/cdrouter.py
 Author: QA Cafe
 Author-email: support@qacafe.com
 License: MIT
 Description: cdrouter
         ========
```


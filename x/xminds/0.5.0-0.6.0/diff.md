# Comparing `tmp/xminds-0.5.0.tar.gz` & `tmp/xminds-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xminds-0.5.0.tar", last modified: Wed Feb 15 23:59:25 2023, max compression
+gzip compressed data, was "dist/xminds-0.6.0.tar", last modified: Wed Apr 19 02:31:20 2023, max compression
```

## Comparing `xminds-0.5.0.tar` & `xminds-0.6.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-02-15 23:59:25.000000 xminds-0.5.0/
--rw-r--r--   0 emile      (502) staff       (20)      750 2023-02-15 23:59:25.000000 xminds-0.5.0/PKG-INFO
--rw-r--r--   0 emile      (502) staff       (20)      289 2021-03-06 05:56:48.000000 xminds-0.5.0/README.rst
--rw-r--r--   0 emile      (502) staff       (20)       38 2023-02-15 23:59:25.000000 xminds-0.5.0/setup.cfg
--rw-r--r--   0 emile      (502) staff       (20)     1141 2021-09-29 16:05:53.000000 xminds-0.5.0/setup.py
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-02-15 23:59:25.000000 xminds-0.5.0/xminds/
--rw-r--r--   0 emile      (502) staff       (20)       77 2023-02-15 23:58:55.000000 xminds-0.5.0/xminds/__init__.py
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-02-15 23:59:25.000000 xminds-0.5.0/xminds/_lib/
--rw-r--r--   0 emile      (502) staff       (20)        0 2021-03-06 05:56:48.000000 xminds-0.5.0/xminds/_lib/__init__.py
--rw-r--r--   0 emile      (502) staff       (20)      937 2021-03-06 05:56:48.000000 xminds-0.5.0/xminds/_lib/compat.py
--rw-r--r--   0 emile      (502) staff       (20)    30299 2021-09-29 16:05:53.000000 xminds-0.5.0/xminds/_lib/hashmap.py
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-02-15 23:59:25.000000 xminds-0.5.0/xminds/api/
--rw-r--r--   0 emile      (502) staff       (20)      184 2021-03-06 05:56:48.000000 xminds-0.5.0/xminds/api/__init__.py
--rw-r--r--   0 emile      (502) staff       (20)     5420 2023-01-05 20:11:10.000000 xminds-0.5.0/xminds/api/apirequest.py
--rw-r--r--   0 emile      (502) staff       (20)   103039 2023-02-15 23:58:25.000000 xminds-0.5.0/xminds/api/client.py
--rw-r--r--   0 emile      (502) staff       (20)     3109 2022-08-23 22:05:50.000000 xminds-0.5.0/xminds/api/exceptions.py
--rw-r--r--   0 emile      (502) staff       (20)      517 2021-03-06 05:56:48.000000 xminds-0.5.0/xminds/compat.py
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-02-15 23:59:25.000000 xminds-0.5.0/xminds/ds/
--rw-r--r--   0 emile      (502) staff       (20)       47 2021-03-06 05:56:48.000000 xminds-0.5.0/xminds/ds/__init__.py
--rw-r--r--   0 emile      (502) staff       (20)     2875 2021-03-06 05:56:48.000000 xminds-0.5.0/xminds/ds/scaling.py
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-02-15 23:59:25.000000 xminds-0.5.0/xminds/lib/
--rw-r--r--   0 emile      (502) staff       (20)       53 2021-03-06 05:56:48.000000 xminds-0.5.0/xminds/lib/__init__.py
--rw-r--r--   0 emile      (502) staff       (20)    23723 2022-01-27 18:13:19.000000 xminds-0.5.0/xminds/lib/aggregate.py
--rw-r--r--   0 emile      (502) staff       (20)     8506 2022-01-27 18:13:19.000000 xminds-0.5.0/xminds/lib/arraybase.py
--rw-r--r--   0 emile      (502) staff       (20)    17756 2021-09-29 16:05:53.000000 xminds-0.5.0/xminds/lib/arrays.py
--rw-r--r--   0 emile      (502) staff       (20)     4080 2021-03-06 05:56:48.000000 xminds-0.5.0/xminds/lib/iterable.py
--rw-r--r--   0 emile      (502) staff       (20)     8594 2021-03-06 05:56:48.000000 xminds-0.5.0/xminds/lib/utils.py
-drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-02-15 23:59:25.000000 xminds-0.5.0/xminds.egg-info/
--rw-r--r--   0 emile      (502) staff       (20)      750 2023-02-15 23:59:25.000000 xminds-0.5.0/xminds.egg-info/PKG-INFO
--rw-r--r--   0 emile      (502) staff       (20)      545 2023-02-15 23:59:25.000000 xminds-0.5.0/xminds.egg-info/SOURCES.txt
--rw-r--r--   0 emile      (502) staff       (20)        1 2023-02-15 23:59:25.000000 xminds-0.5.0/xminds.egg-info/dependency_links.txt
--rw-r--r--   0 emile      (502) staff       (20)       29 2023-02-15 23:59:25.000000 xminds-0.5.0/xminds.egg-info/requires.txt
--rw-r--r--   0 emile      (502) staff       (20)        7 2023-02-15 23:59:25.000000 xminds-0.5.0/xminds.egg-info/top_level.txt
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/
+-rw-r--r--   0 emile      (502) staff       (20)      750 2023-04-19 02:31:20.000000 xminds-0.6.0/PKG-INFO
+-rw-r--r--   0 emile      (502) staff       (20)      289 2021-03-06 05:56:48.000000 xminds-0.6.0/README.rst
+-rw-r--r--   0 emile      (502) staff       (20)       38 2023-04-19 02:31:20.000000 xminds-0.6.0/setup.cfg
+-rw-r--r--   0 emile      (502) staff       (20)     1141 2021-09-29 16:05:53.000000 xminds-0.6.0/setup.py
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds/
+-rw-r--r--   0 emile      (502) staff       (20)       77 2023-04-19 02:29:24.000000 xminds-0.6.0/xminds/__init__.py
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds/_lib/
+-rw-r--r--   0 emile      (502) staff       (20)        0 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/_lib/__init__.py
+-rw-r--r--   0 emile      (502) staff       (20)      937 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/_lib/compat.py
+-rw-r--r--   0 emile      (502) staff       (20)    30299 2021-09-29 16:05:53.000000 xminds-0.6.0/xminds/_lib/hashmap.py
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds/api/
+-rw-r--r--   0 emile      (502) staff       (20)      184 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/api/__init__.py
+-rw-r--r--   0 emile      (502) staff       (20)     5537 2023-04-19 02:29:24.000000 xminds-0.6.0/xminds/api/apirequest.py
+-rw-r--r--   0 emile      (502) staff       (20)   106531 2023-04-19 02:29:24.000000 xminds-0.6.0/xminds/api/client.py
+-rw-r--r--   0 emile      (502) staff       (20)     3109 2022-08-23 22:05:50.000000 xminds-0.6.0/xminds/api/exceptions.py
+-rw-r--r--   0 emile      (502) staff       (20)      517 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/compat.py
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds/ds/
+-rw-r--r--   0 emile      (502) staff       (20)       47 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/ds/__init__.py
+-rw-r--r--   0 emile      (502) staff       (20)     2875 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/ds/scaling.py
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds/lib/
+-rw-r--r--   0 emile      (502) staff       (20)       53 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/lib/__init__.py
+-rw-r--r--   0 emile      (502) staff       (20)    23723 2022-01-27 18:13:19.000000 xminds-0.6.0/xminds/lib/aggregate.py
+-rw-r--r--   0 emile      (502) staff       (20)     8506 2022-01-27 18:13:19.000000 xminds-0.6.0/xminds/lib/arraybase.py
+-rw-r--r--   0 emile      (502) staff       (20)    17756 2021-09-29 16:05:53.000000 xminds-0.6.0/xminds/lib/arrays.py
+-rw-r--r--   0 emile      (502) staff       (20)     4080 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/lib/iterable.py
+-rw-r--r--   0 emile      (502) staff       (20)     8594 2021-03-06 05:56:48.000000 xminds-0.6.0/xminds/lib/utils.py
+drwxr-xr-x   0 emile      (502) staff       (20)        0 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds.egg-info/
+-rw-r--r--   0 emile      (502) staff       (20)      750 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds.egg-info/PKG-INFO
+-rw-r--r--   0 emile      (502) staff       (20)      545 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds.egg-info/SOURCES.txt
+-rw-r--r--   0 emile      (502) staff       (20)        1 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds.egg-info/dependency_links.txt
+-rw-r--r--   0 emile      (502) staff       (20)       29 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds.egg-info/requires.txt
+-rw-r--r--   0 emile      (502) staff       (20)        7 2023-04-19 02:31:20.000000 xminds-0.6.0/xminds.egg-info/top_level.txt
```

### Comparing `xminds-0.5.0/PKG-INFO` & `xminds-0.6.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xminds
-Version: 0.5.0
+Version: 0.6.0
 Summary:  Crossing Minds data science python library and API client
 Home-page: https://github.com/Crossing-Minds/xminds-python
 Author: Crossing Minds, Inc
 Author-email: contact@crossingminds.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xminds-0.5.0/setup.py` & `xminds-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `xminds-0.5.0/xminds/_lib/compat.py` & `xminds-0.6.0/xminds/_lib/compat.py`

 * *Files identical despite different names*

### Comparing `xminds-0.5.0/xminds/_lib/hashmap.py` & `xminds-0.6.0/xminds/_lib/hashmap.py`

 * *Files identical despite different names*

### Comparing `xminds-0.5.0/xminds/api/apirequest.py` & `xminds-0.6.0/xminds/api/apirequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     def __init__(self, host=None, api_version=None, headers=None):
         self.host = host or self.HOST
         headers = dict(self.HEADERS, **headers or {})
         self.api_version = api_version or self.API_VERSION
         self.session = requests.Session()
         self.session.headers.update(headers)
         self._jwt_token = None
-        self._last_trace = None
+        self._last_headers = None
 
     def get(self, path, params=None, **kwargs):
         return self._request('GET', path, params=params, **kwargs)
 
     def put(self, path, data, **kwargs):
         return self._request('PUT', path, data=data, **kwargs)
 
@@ -60,16 +60,20 @@
         self._jwt_token = jwt_token
         self.session.headers.update({'Authorization': f'Bearer {jwt_token}'})
 
     def clear_jwt_token(self):
         self.session.headers.pop('Authorization', None)
 
     @property
+    def last_headers(self):
+        return self._last_headers
+
+    @property
     def last_trace(self):
-        return self._last_trace
+        return self._last_headers.get('X-Cloud-Trace-Context')
 
     # ConnectionError means the request didn't reach the server
     # so even POST requests can be retried:
     @retry(base=0.1, multiplier=4, max_retry=3, exception=requests.ConnectionError)  # wait up to ~2s
     def _request(self, method, path, params=None, data=None, timeout=None):
         url = f'{self.host}/{self.api_version}/{path}'
         if path and not path.endswith('/'):
@@ -79,15 +83,17 @@
             'timeout': timeout or self.DEFAULT_TIMEOUT,
             **self._REQUEST_KWARGS
         }
         if data:
             request_kwargs['data'] = self._serialize_data(data)
         if params:
             request_kwargs['params'] = params
+        self._last_headers = None
         resp = self.session.request(method, url, **request_kwargs)
+        self._last_headers = resp.headers
 
         if resp.status_code >= 500:
             exc_payload = self._parse_response(resp, fallback=True)
             if exc_payload:
                 logging.error(exc_payload)
             raise ServerError(exc_payload)
         elif resp.status_code >= 400:
@@ -95,15 +101,14 @@
             try:
                 exc = XMindsError.from_code(data.get('error_code', 0), data.get('error_data'))
             except (KeyError, AttributeError, TypeError, ValueError):
                 exc = ServerError({'response': data})
             raise exc
 
         data = self._parse_response(resp)
-        self._last_trace = resp.headers.get('X-Cloud-Trace-Context')
         return data
 
     def _serialize_data(self, data):
         raise NotImplementedError()
 
     def _parse_response(self, response, fallback=False):
         raise NotImplementedError()
```

### Comparing `xminds-0.5.0/xminds/api/client.py` & `xminds-0.6.0/xminds/api/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -970,22 +970,23 @@
         item_id = self._itemid2url(item_id)
         path = f'items/{item_id}/'
         resp = self.api.get(path=path)
         resp['item']['item_id'] = self._body2itemid(resp['item']['item_id'])
         return resp
 
     @require_login
-    def list_items(self, items_id):
+    def list_items(self, items_id, properties=None):
         """
         Get multiple items given their IDs.
         The items in the response are not aligned with the input.
         In particular this endpoint does not raise NotFoundError if any item in missing.
         Instead, the missing items are simply not present in the response.
 
         :param ID-array items_id: items IDs
+        :param list-of-str? properties: properties to return (default: all)
         :returns: {
             'items': array with fields ['id': ID, *<property_name: value_type>]
                 contains only the non-repeated values,
             'items_m2m': dict of arrays for repeated values:
                 {
                     *<repeated_property_name: {
                         'name': str,
@@ -994,14 +995,16 @@
                 },
             'warnings?': [str],
         }
         """
         items_id = self._itemid2body(items_id)
         path = f'items-bulk/list/'
         data = {'items_id': items_id}
+        if properties is not None:
+            data['properties'] = properties
         resp = self.api.post(path=path, data=data)
         resp['items'] = self._body2itemid(resp['items'])
         return resp
 
     @require_login
     def list_items_paginated(self, amt=None, cursor=None):
         """
@@ -1822,76 +1825,92 @@
         user_id = self._userid2url(user_id)
         path = f'users/{user_id}/ratings/'
         return self.api.delete(path=path)
 
     # === User Interactions ===
 
     @require_login
-    def create_interaction(self, user_id, item_id, interaction_type, timestamp=None):
+    def create_interaction(self, user_id, item_id, interaction_type, timestamp=None,
+                           properties=None):
         """
         This endpoint allows you to create a new interaction for a user and an item.
         An inferred rating will be created or updated for the tuple (user_id, item_id).
         The taste profile of the user will then be updated in real-time by the online machine learning algorithm.
 
         Note: replace `user_id` with `AUTO_FRONTEND_ID` variable when call the method to use the
         value inside the JWT. Only for FRONTEND role. For instance: `method(AUTO_FRONTEND_ID, ...)`
 
         :param ID user_id: user ID
         :param ID item_id: item ID
         :param str interaction_type: Interaction type
         :param float? timestamp: rating timestamp (default: now)
+        :param dict? properties: interaction properties {prop_name: prop_value)
+        :returns: {
+            'warnings': [str],
+        }
         """
         user_id = self._userid2url(user_id)
         item_id = self._itemid2url(item_id)
         path = f'users/{user_id}/interactions/{item_id}/'
         data = {
             'interaction_type': interaction_type,
         }
         if timestamp is not None:
             data['timestamp'] = timestamp
+        if properties is not None:
+            data['properties'] = properties
         return self.api.post(path=path, data=data)
 
     @require_login
     def create_interactions_bulk(self, interactions, chunk_size=(1 << 14)):
         """
         Create or update large bulks of interactions for many users and many items.
         Inferred ratings will be created or updated for all tuples (user_id, item_id).
 
         :param array interactions: interactions array with fields:
-            ['user_id': ID, 'item_id': ID, 'interaction_type': str, 'timestamp': float]
+            ['user_id': ID, 'item_id': ID, 'interaction_type': str, 'timestamp': float,
+             'properties?': nested numpy.ndarray with fields [prop_name: prop_value, ...] ]
         :param int? chunk_size: split the requests in chunks of this size (default: 16_000)
+        :returns: {
+            'warnings': [str],
+        }
         """
         path = f'interactions-bulk/'
         n_chunks = int(numpy.ceil(len(interactions) / chunk_size))
         sleep = chunk_size / 500
+        warnings = []
         for i in tqdm(range(n_chunks), disable=(True if n_chunks < 4 else None)):
             interactions_chunk = interactions[i*chunk_size:(i+1)*chunk_size]
             interactions_chunk = self._userid2body(self._itemid2body(interactions_chunk))
             data = {
                 'interactions': interactions_chunk,
             }
-            self.api.post(path=path, data=data, timeout=10)
+            resp = self.api.post(path=path, data=data, timeout=10)
+            warnings += [resp.get('warnings', [])]
             if n_chunks > 1:
                 time.sleep(sleep)
-
-        return
+        return {'warnings': warnings}
 
     @require_login
     def create_user_interactions_bulk(self, user_id, interactions):
         """
         Create a small bulk of interactions for a single user and many items.
         Inferred ratings will be created or updated for all tuples (user_id, item_id)
 
         Note: replace `user_id` with `AUTO_FRONTEND_ID` variable when call the method to use the
         value inside the JWT. Only for FRONTEND role. For instance: `method(AUTO_FRONTEND_ID, ...)`
 
         :param ID user_id: user ID
         :param array interactions: interactions array with fields:
-            ['item_id': ID, 'interaction_type': str, 'timestamp': float]
+            ['item_id': ID, 'interaction_type': str, 'timestamp': float,
+             'properties?': nested numpy.ndarray with fields [prop_name: prop_value, ...] ]
         :param int? chunk_size: split the requests in chunks of this size (default: 16_000)
+        :returns: {
+            'warnings': [str],
+        }
         """
         user_id = self._userid2url(user_id)
         path = f'users/{user_id}/interactions-bulk/'
         data = {
             'interactions': interactions,
         }
         return self.api.post(path=path, data=data, timeout=10)
@@ -1910,15 +1929,16 @@
             timestamped after this value
         :param float? end_timestamp: When provided, only returns interactions
             timestamped before this value
         :returns: {
             'has_next': bool,
             'next_cursor': str,
             'interactions': array with fields
-                ['item_id': ID, 'user_id': ID, 'interaction_type': str, 'timestamp': float]
+                ['item_id': ID, 'user_id': ID, 'interaction_type': str, 'timestamp': float,
+                 'properties?': nested numpy.ndarray with fields [prop_name: prop_value, ...] ]
             'warnings?': [str],
         }
         :raises: RequestError if provided timeframe is invalid
         """
         path = f'interactions-bulk/'
         params = {}
         if amt is not None:
@@ -1929,52 +1949,86 @@
             params['start_timestamp'] = start_timestamp
         if end_timestamp:
             params['end_timestamp'] = end_timestamp
         resp = self.api.get(path=path, params=params)
         resp['interactions'] = self._body2userid(self._body2itemid(resp['interactions']))
         return resp
 
+    @require_login
+    def list_user_interactions(
+            self, user_id, amt=None, cursor=None,
+    ):
+        """
+        List the interactions of one user
+
+        :param int? amt: amount to return (default: use the API default)
+        :param str? cursor: Pagination cursor
+        :returns: {
+            'has_next': bool,
+            'next_cursor': str,
+            'interactions': array with fields
+                ['item_id': ID, 'interaction_type': str, 'timestamp': float,
+                 'properties?': nested numpy.ndarray with fields [prop_name: prop_value, ...] ]
+            'warnings?': [str],
+        }
+        """
+        user_id = self._userid2url(user_id)
+        path = f'users/{user_id}/interactions-bulk/'
+        params = {}
+        if amt is not None:
+            params['amt'] = amt
+        if cursor:
+            params['cursor'] = cursor
+        resp = self.api.get(path=path, params=params)
+        resp['interactions'] = self._body2itemid(resp['interactions'])
+        return resp
+
     # === Session Interactions ===
 
     @require_login
-    def create_session_interaction(self, session_id, item_id, interaction_type, timestamp=None):
+    def create_session_interaction(self, session_id, item_id, interaction_type, timestamp=None,
+                                   properties=None):
         """
         This endpoint allows you to create a new interaction for an anonymous session and an item.
 
         Note: replace `session_id` with `AUTO_FRONTEND_ID` variable when call the method to use the
         value inside the JWT. Only for FRONTEND role. For instance: `method(AUTO_FRONTEND_ID, ...)`
 
         :param ID session_id: anonymous session ID
         :param ID item_id: item ID
         :param str interaction_type: Interaction type
         :param float? timestamp: rating timestamp (default: now)
+        :param dict? properties:
         :returns: {
-            'warnings?': [str],
+            'warnings': [str],
         }
         """
         session_id = self._sessionid2url(session_id)
         item_id = self._itemid2url(item_id)
         path = f'sessions/{session_id}/items/{item_id}/interactions/'
         data = {
             'interaction_type': interaction_type,
         }
         if timestamp is not None:
             data['timestamp'] = timestamp
+        if properties is not None:
+            data['properties'] = properties
         return self.api.post(path=path, data=data)
 
     @require_login
     def create_sessions_interactions_bulk(self, interactions, chunk_size=(1 << 14)):
         """
         Create or update large bulks of interactions for many anonymous session and many items.
 
         :param array interactions: interactions array with fields:
-            ['session_id': ID, 'item_id': ID, 'interaction_type': str, 'timestamp': float]
+            ['session_id': ID, 'item_id': ID, 'interaction_type': str, 'timestamp': float,
+             'properties?': numpy.ndarray ]
         :param int? chunk_size: split the requests in chunks of this size (default: 16_000)
         :returns: {
-            'warnings?': [str],
+            'warnings': [str],
         }
         """
         path = f'sessions-interactions-bulk/'
         n_chunks = int(numpy.ceil(len(interactions) / chunk_size))
         sleep = chunk_size / 500
         warnings = []
         for i in tqdm(range(n_chunks), disable=(True if n_chunks < 4 else None)):
@@ -1995,15 +2049,16 @@
         Create a small bulk of interactions for a single anonymous session and many items.
 
         Note: replace `session_id` with `AUTO_FRONTEND_ID` variable when call the method to use the
         value inside the JWT. Only for FRONTEND role. For instance: `method(AUTO_FRONTEND_ID, ...)`
 
         :param ID session_id: anonymous session ID
         :param array interactions: interactions array with fields:
-            ['item_id': ID, 'interaction_type': str, 'timestamp': float]
+            ['item_id': ID, 'interaction_type': str, 'timestamp': float,
+             'properties?': nested numpy.ndarray with fields [prop_name: prop_value, ...] ]
         :param int? chunk_size: split the requests in chunks of this size (default: 16_000)
         :returns: {
             'warnings?': [str],
         }
         """
         session_id = self._sessionid2url(session_id)
         path = f'sessions/{session_id}/interactions-bulk/'
@@ -2026,15 +2081,16 @@
             timestamped after this value
         :param float? end_timestamp: When provided, only returns interactions
             timestamped before this value
         :returns: {
             'has_next': bool,
             'next_cursor': str,
             'interactions': array with fields
-                ['item_id': ID, 'session_id': ID, 'interaction_type': str, 'timestamp': float]
+                ['item_id': ID, 'session_id': ID, 'interaction_type': str, 'timestamp': float,
+                'properties?': nested numpy.ndarray with fields [prop_name: prop_value, ...] ]
             'warnings?': [str],
         }
         :raises: RequestError if provided timeframe is invalid
         """
         path = f'sessions-interactions-bulk/'
         params = {}
         if amt is not None:
@@ -2046,14 +2102,43 @@
         if end_timestamp:
             params['end_timestamp'] = end_timestamp
         resp = self.api.get(path=path, params=params)
         resp['interactions'] = self._body2sessionid(self._body2itemid(resp['interactions']))
         return resp
 
     @require_login
+    def list_session_interactions(
+            self, session_id, amt=None, cursor=None,
+    ):
+        """
+        List the interactions of one anonymous session
+
+        :param ID session_id:
+        :param int? amt: amount to return (default: use the API default)
+        :param str? cursor: Pagination cursor
+        :returns: {
+            'has_next': bool,
+            'next_cursor': str,
+            'interactions': array with fields
+                ['item_id': ID, 'interaction_type': str, 'timestamp': float,
+                 'properties?': nested numpy.ndarray with fields [prop_name: prop_value, ...] ]
+            'warnings?': [str],
+        }
+        """
+        session_id = self._sessionid2url(session_id)
+        path = f'sessions/{session_id}/interactions-bulk/'
+        params = {}
+        if amt is not None:
+            params['amt'] = amt
+        if cursor:
+            params['cursor'] = cursor
+        resp = self.api.get(path=path, params=params)
+        resp['interactions'] = self._body2itemid(resp['interactions'])
+        return resp
+
     def resolve_session(self, user_id, session_id, timestamp=None):
         """
         This endpoint allows you to resolve an anonymous session with a user.
         Note: one user can have many anonymous sessions.
 
         :param ID user_id:
         :param ID session_id:
@@ -2513,14 +2598,18 @@
         return self.api.clear_jwt_token()
 
     @property
     def jwt_token(self):
         return self.api.jwt_token
 
     @property
+    def last_headers(self):
+        return self.api.last_headers
+
+    @property
     def last_trace(self):
         return self.api.last_trace
 
     def set_jwt_token(self, jwt_token):
         self.api.set_jwt_token(jwt_token)
 
     def escape_url(self, param):
```

### Comparing `xminds-0.5.0/xminds/api/exceptions.py` & `xminds-0.6.0/xminds/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `xminds-0.5.0/xminds/compat.py` & `xminds-0.6.0/xminds/compat.py`

 * *Files identical despite different names*

### Comparing `xminds-0.5.0/xminds/ds/scaling.py` & `xminds-0.6.0/xminds/ds/scaling.py`

 * *Files identical despite different names*

### Comparing `xminds-0.5.0/xminds/lib/aggregate.py` & `xminds-0.6.0/xminds/lib/aggregate.py`

 * *Files identical despite different names*

### Comparing `xminds-0.5.0/xminds/lib/arraybase.py` & `xminds-0.6.0/xminds/lib/arraybase.py`

 * *Files identical despite different names*

### Comparing `xminds-0.5.0/xminds/lib/arrays.py` & `xminds-0.6.0/xminds/lib/arrays.py`

 * *Files identical despite different names*

### Comparing `xminds-0.5.0/xminds/lib/iterable.py` & `xminds-0.6.0/xminds/lib/iterable.py`

 * *Files identical despite different names*

### Comparing `xminds-0.5.0/xminds/lib/utils.py` & `xminds-0.6.0/xminds/lib/utils.py`

 * *Files identical despite different names*

### Comparing `xminds-0.5.0/xminds.egg-info/PKG-INFO` & `xminds-0.6.0/xminds.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xminds
-Version: 0.5.0
+Version: 0.6.0
 Summary:  Crossing Minds data science python library and API client
 Home-page: https://github.com/Crossing-Minds/xminds-python
 Author: Crossing Minds, Inc
 Author-email: contact@crossingminds.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xminds-0.5.0/xminds.egg-info/SOURCES.txt` & `xminds-0.6.0/xminds.egg-info/SOURCES.txt`

 * *Files identical despite different names*


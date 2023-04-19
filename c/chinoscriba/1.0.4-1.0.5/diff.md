# Comparing `tmp/chinoscriba-1.0.4.tar.gz` & `tmp/chinoscriba-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chinoscriba-1.0.4.tar", last modified: Tue May 18 13:23:34 2021, max compression
+gzip compressed data, was "chinoscriba-1.0.5.tar", last modified: Wed Apr 19 10:22:02 2023, max compression
```

## Comparing `chinoscriba-1.0.4.tar` & `chinoscriba-1.0.5.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 13:23:34.000000 chinoscriba-1.0.4/
--rw-r--r--   0 root         (0) root         (0)     4512 2021-05-18 13:23:34.000000 chinoscriba-1.0.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3181 2021-05-05 09:47:55.000000 chinoscriba-1.0.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 13:23:34.000000 chinoscriba-1.0.4/chinoscriba/
--rw-r--r--   0 root         (0) root         (0)     1377 2021-05-18 13:23:33.000000 chinoscriba-1.0.4/chinoscriba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 13:23:34.000000 chinoscriba-1.0.4/chinoscriba/api/
--rw-r--r--   0 root         (0) root         (0)      277 2021-05-18 13:23:33.000000 chinoscriba-1.0.4/chinoscriba/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8181 2021-05-18 13:23:32.000000 chinoscriba-1.0.4/chinoscriba/api/blocks_api.py
--rw-r--r--   0 root         (0) root         (0)    25287 2021-05-18 13:23:32.000000 chinoscriba-1.0.4/chinoscriba/api/events_api.py
--rw-r--r--   0 root         (0) root         (0)    17137 2021-05-18 13:23:32.000000 chinoscriba-1.0.4/chinoscriba/api/logs_api.py
--rw-r--r--   0 root         (0) root         (0)     4657 2021-05-18 13:23:32.000000 chinoscriba-1.0.4/chinoscriba/api/stats_api.py
--rw-r--r--   0 root         (0) root         (0)    24814 2021-05-18 13:23:33.000000 chinoscriba-1.0.4/chinoscriba/api_client.py
--rw-r--r--   0 root         (0) root         (0)     8534 2021-05-18 13:23:33.000000 chinoscriba-1.0.4/chinoscriba/configuration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 13:23:34.000000 chinoscriba-1.0.4/chinoscriba/models/
--rw-r--r--   0 root         (0) root         (0)     1041 2021-05-18 13:23:33.000000 chinoscriba-1.0.4/chinoscriba/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14568 2021-05-18 13:23:29.000000 chinoscriba-1.0.4/chinoscriba/models/audit_log.py
--rw-r--r--   0 root         (0) root         (0)    11485 2021-05-18 13:23:30.000000 chinoscriba-1.0.4/chinoscriba/models/block.py
--rw-r--r--   0 root         (0) root         (0)     7000 2021-05-18 13:23:30.000000 chinoscriba-1.0.4/chinoscriba/models/event.py
--rw-r--r--   0 root         (0) root         (0)     5253 2021-05-18 13:23:30.000000 chinoscriba-1.0.4/chinoscriba/models/inline_response200.py
--rw-r--r--   0 root         (0) root         (0)     5273 2021-05-18 13:23:30.000000 chinoscriba-1.0.4/chinoscriba/models/inline_response2001.py
--rw-r--r--   0 root         (0) root         (0)     5267 2021-05-18 13:23:31.000000 chinoscriba-1.0.4/chinoscriba/models/inline_response2002.py
--rw-rw-rw-   0 root         (0) root         (0)     5150 2021-03-10 12:21:22.000000 chinoscriba-1.0.4/chinoscriba/models/inline_response200_bis.py
--rw-r--r--   0 root         (0) root         (0)    16827 2021-05-18 13:23:31.000000 chinoscriba-1.0.4/chinoscriba/models/log.py
--rw-r--r--   0 root         (0) root         (0)     3362 2021-05-18 13:23:31.000000 chinoscriba-1.0.4/chinoscriba/models/multi_audit_log_serializer_output.py
--rw-r--r--   0 root         (0) root         (0)     3803 2021-05-18 13:23:31.000000 chinoscriba-1.0.4/chinoscriba/models/search_request.py
--rw-r--r--   0 root         (0) root         (0)     4075 2021-05-18 13:23:31.000000 chinoscriba-1.0.4/chinoscriba/models/sort_rule.py
--rw-r--r--   0 root         (0) root         (0)     8028 2021-05-18 13:23:31.000000 chinoscriba-1.0.4/chinoscriba/models/stat.py
--rw-r--r--   0 root         (0) root         (0)    13250 2021-05-18 13:23:33.000000 chinoscriba-1.0.4/chinoscriba/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 13:23:34.000000 chinoscriba-1.0.4/chinoscriba.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4512 2021-05-18 13:23:34.000000 chinoscriba-1.0.4/chinoscriba.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      945 2021-05-18 13:23:34.000000 chinoscriba-1.0.4/chinoscriba.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-05-18 13:23:34.000000 chinoscriba-1.0.4/chinoscriba.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2021-05-18 13:23:34.000000 chinoscriba-1.0.4/chinoscriba.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2021-05-18 13:23:34.000000 chinoscriba-1.0.4/chinoscriba.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-05-18 13:23:34.000000 chinoscriba-1.0.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1318 2021-05-18 13:23:33.000000 chinoscriba-1.0.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-05-18 13:23:34.000000 chinoscriba-1.0.4/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2021-03-10 12:21:22.000000 chinoscriba-1.0.4/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17533 2021-05-06 11:05:21.000000 chinoscriba-1.0.4/test/test_default_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)     3621 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3181 2022-08-24 15:25:53.000000 chinoscriba-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 10:22:02.383192 chinoscriba-1.0.5/chinoscriba/
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/chinoscriba/api/
+-rw-r--r--   0 root         (0) root         (0)      277 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8189 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/api/blocks_api.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/api/events_api.py
+-rw-r--r--   0 root         (0) root         (0)    25634 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/api/logs_api.py
+-rw-r--r--   0 root         (0) root         (0)     7718 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/api/stats_api.py
+-rw-r--r--   0 root         (0) root         (0)    24814 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba/api_client.py
+-rw-r--r--   0 root         (0) root         (0)     8796 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba/configuration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/chinoscriba/models/
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14568 2023-04-19 10:22:00.000000 chinoscriba-1.0.5/chinoscriba/models/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)    11485 2023-04-19 10:22:00.000000 chinoscriba-1.0.5/chinoscriba/models/block.py
+-rw-r--r--   0 root         (0) root         (0)     7000 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/event.py
+-rw-r--r--   0 root         (0) root         (0)     5253 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/inline_response200.py
+-rw-r--r--   0 root         (0) root         (0)     5273 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/inline_response2001.py
+-rw-r--r--   0 root         (0) root         (0)     5267 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/inline_response2002.py
+-rw-rw-rw-   0 root         (0) root         (0)     5150 2022-08-24 15:25:53.000000 chinoscriba-1.0.5/chinoscriba/models/inline_response200_bis.py
+-rw-r--r--   0 root         (0) root         (0)    16827 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/log.py
+-rw-r--r--   0 root         (0) root         (0)     3362 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/multi_audit_log_serializer_output.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/search_request.py
+-rw-r--r--   0 root         (0) root         (0)     4075 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/sort_rule.py
+-rw-r--r--   0 root         (0) root         (0)     8028 2023-04-19 10:22:01.000000 chinoscriba-1.0.5/chinoscriba/models/stat.py
+-rw-rw-rw-   0 root         (0) root         (0)    13815 2023-04-19 09:49:35.000000 chinoscriba-1.0.5/chinoscriba/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/chinoscriba.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3621 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      959 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/chinoscriba.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2023-04-19 10:22:02.000000 chinoscriba-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 10:22:02.387193 chinoscriba-1.0.5/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-08-24 15:25:53.000000 chinoscriba-1.0.5/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18730 2022-08-24 15:25:53.000000 chinoscriba-1.0.5/test/test_default_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1316 2022-08-24 15:25:53.000000 chinoscriba-1.0.5/test/utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `chinoscriba-1.0.4/README.md` & `chinoscriba-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/__init__.py` & `chinoscriba-1.0.5/chinoscriba/__init__.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/api/blocks_api.py` & `chinoscriba-1.0.5/chinoscriba/api/blocks_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['Basic', 'BearerJwt']  # noqa: E501
+        auth_settings = ['Basic', 'InternalToken']  # noqa: E501
 
         return self.api_client.call_api(
             '/exported/', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -200,15 +200,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['Basic', 'BearerJwt']  # noqa: E501
+        auth_settings = ['Basic', 'InternalToken']  # noqa: E501
 
         return self.api_client.call_api(
             '/exported/{block_id}', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `chinoscriba-1.0.4/chinoscriba/api/events_api.py` & `chinoscriba-1.0.5/chinoscriba/api/events_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['Basic', 'BearerJwt']  # noqa: E501
+        auth_settings = ['Basic', 'InternalToken']  # noqa: E501
 
         return self.api_client.call_api(
             '/events/', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -200,15 +200,15 @@
         header_params = {}
 
         form_params = []
         local_var_files = {}
 
         body_params = None
         # Authentication setting
-        auth_settings = ['Basic', 'BearerJwt']  # noqa: E501
+        auth_settings = ['Basic', 'InternalToken']  # noqa: E501
 
         return self.api_client.call_api(
             '/events/{event_id}/', 'DELETE',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -295,15 +295,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['Basic', 'BearerJwt']  # noqa: E501
+        auth_settings = ['Basic', 'InternalToken']  # noqa: E501
 
         return self.api_client.call_api(
             '/events/', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -402,15 +402,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['Basic', 'BearerJwt']  # noqa: E501
+        auth_settings = ['Basic', 'InternalToken']  # noqa: E501
 
         return self.api_client.call_api(
             '/events/{event_id}/', 'PATCH',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -497,15 +497,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['Basic', 'BearerJwt']  # noqa: E501
+        auth_settings = ['Basic', 'InternalToken']  # noqa: E501
 
         return self.api_client.call_api(
             '/events/{event_id}/', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -604,15 +604,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['Basic', 'BearerJwt']  # noqa: E501
+        auth_settings = ['Basic', 'InternalToken']  # noqa: E501
 
         return self.api_client.call_api(
             '/events/{event_id}/', 'PUT',
             path_params,
             query_params,
             header_params,
             body=body_params,
```

### Comparing `chinoscriba-1.0.4/chinoscriba/api/logs_api.py` & `chinoscriba-1.0.5/chinoscriba/api/logs_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['Basic', 'BearerJwt']  # noqa: E501
+        auth_settings = ['Basic', 'InternalToken']  # noqa: E501
 
         return self.api_client.call_api(
             '/logs/', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -208,15 +208,15 @@
 
         body_params = None
         # HTTP header `Accept`
         header_params['Accept'] = self.api_client.select_header_accept(
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['Basic', 'BearerJwt']  # noqa: E501
+        auth_settings = ['Basic', 'InternalToken']  # noqa: E501
 
         return self.api_client.call_api(
             '/logs/', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -307,15 +307,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['Basic', 'BearerJwt']  # noqa: E501
+        auth_settings = ['Basic', 'InternalToken']  # noqa: E501
 
         return self.api_client.call_api(
             '/logs/_multiple/', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -414,15 +414,15 @@
             ['application/json'])  # noqa: E501
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
-        auth_settings = ['Basic', 'BearerJwt']  # noqa: E501
+        auth_settings = ['Basic', 'InternalToken']  # noqa: E501
 
         return self.api_client.call_api(
             '/search/', 'POST',
             path_params,
             query_params,
             header_params,
             body=body_params,
@@ -431,7 +431,205 @@
             response_type='InlineResponse2002',  # noqa: E501
             auth_settings=auth_settings,
             async_req=params.get('async_req'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', True),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
+
+    def me_logs_create(self, body, **kwargs):  # noqa: E501
+        """User - Create a new Log  # noqa: E501
+
+        Submit a new immutable Audit Log with custom values. This is an OAuth only endpoint. The data from the current customer will be set in the system log generated by Scriba (`caller_id`). This does not include the log you are actually creating by calling this endpoint.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.me_logs_create(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param AuditLog body: (required)
+        :return: AuditLog
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.me_logs_create_with_http_info(body, **kwargs)  # noqa: E501
+        else:
+            (data) = self.me_logs_create_with_http_info(body, **kwargs)  # noqa: E501
+            return data
+
+    def me_logs_create_with_http_info(self, body, **kwargs):  # noqa: E501
+        """User - Create a new Log  # noqa: E501
+
+        Submit a new immutable Audit Log with custom values. This is an OAuth only endpoint. The data from the current customer will be set in the system log generated by Scriba (`caller_id`). This does not include the log you are actually creating by calling this endpoint.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.me_logs_create_with_http_info(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param AuditLog body: (required)
+        :return: AuditLog
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method me_logs_create" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `me_logs_create`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerOAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/me/logs', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='AuditLog',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
+
+    def me_logs_multiple(self, body, **kwargs):  # noqa: E501
+        """User - Create multiple Logs (bulk)  # noqa: E501
+
+        Submit a LIST of new immutable Audit Log with custom values. This is an OAuth only endpoint. The data from the current customer will be set in the system log generated by Scriba (`caller_id`). This does not include the log you are actually creating by calling this endpoint.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.me_logs_multiple(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param list[AuditLog] body: (required)
+        :return: MultiAuditLogSerializerOutput
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+        kwargs['_return_http_data_only'] = True
+        if kwargs.get('async_req'):
+            return self.me_logs_multiple_with_http_info(body, **kwargs)  # noqa: E501
+        else:
+            (data) = self.me_logs_multiple_with_http_info(body, **kwargs)  # noqa: E501
+            return data
+
+    def me_logs_multiple_with_http_info(self, body, **kwargs):  # noqa: E501
+        """User - Create multiple Logs (bulk)  # noqa: E501
+
+        Submit a LIST of new immutable Audit Log with custom values. This is an OAuth only endpoint. The data from the current customer will be set in the system log generated by Scriba (`caller_id`). This does not include the log you are actually creating by calling this endpoint.  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+        >>> thread = api.me_logs_multiple_with_http_info(body, async_req=True)
+        >>> result = thread.get()
+
+        :param async_req bool
+        :param list[AuditLog] body: (required)
+        :return: MultiAuditLogSerializerOutput
+                 If the method is called asynchronously,
+                 returns the request thread.
+        """
+
+        all_params = ['body']  # noqa: E501
+        all_params.append('async_req')
+        all_params.append('_return_http_data_only')
+        all_params.append('_preload_content')
+        all_params.append('_request_timeout')
+
+        params = locals()
+        for key, val in six.iteritems(params['kwargs']):
+            if key not in all_params:
+                raise TypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method me_logs_multiple" % key
+                )
+            params[key] = val
+        del params['kwargs']
+        # verify the required parameter 'body' is set
+        if ('body' not in params or
+                params['body'] is None):
+            raise ValueError("Missing the required parameter `body` when calling `me_logs_multiple`")  # noqa: E501
+
+        collection_formats = {}
+
+        path_params = {}
+
+        query_params = []
+
+        header_params = {}
+
+        form_params = []
+        local_var_files = {}
+
+        body_params = None
+        if 'body' in params:
+            body_params = params['body']
+        # HTTP header `Accept`
+        header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # HTTP header `Content-Type`
+        header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
+            ['application/json'])  # noqa: E501
+
+        # Authentication setting
+        auth_settings = ['BearerOAuth']  # noqa: E501
+
+        return self.api_client.call_api(
+            '/me/logs/_multiple', 'POST',
+            path_params,
+            query_params,
+            header_params,
+            body=body_params,
+            post_params=form_params,
+            files=local_var_files,
+            response_type='MultiAuditLogSerializerOutput',  # noqa: E501
+            auth_settings=auth_settings,
+            async_req=params.get('async_req'),
+            _return_http_data_only=params.get('_return_http_data_only'),
+            _preload_content=params.get('_preload_content', True),
+            _request_timeout=params.get('_request_timeout'),
+            collection_formats=collection_formats)
```

### Comparing `chinoscriba-1.0.4/chinoscriba/api_client.py` & `chinoscriba-1.0.5/chinoscriba/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/1.0.4/python'
+        self.user_agent = 'Swagger-Codegen/1.0.5/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `chinoscriba-1.0.4/chinoscriba/configuration.py` & `chinoscriba-1.0.5/chinoscriba/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,15 +232,22 @@
             'Basic':
                 {
                     'type': 'basic',
                     'in': 'header',
                     'key': 'Authorization',
                     'value': self.get_basic_auth_token()
                 },
-            'BearerJwt':
+            'BearerOAuth':
+                {
+                    'type': 'api_key',
+                    'in': 'header',
+                    'key': 'Authorization',
+                    'value': self.get_api_key_with_prefix('Authorization')
+                },
+            'InternalToken':
                 {
                     'type': 'api_key',
                     'in': 'header',
                     'key': 'Authorization',
                     'value': self.get_api_key_with_prefix('Authorization')
                 },
         }
@@ -250,9 +257,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: v1\n"\
-               "SDK Package Version: 1.0.4".\
+               "SDK Package Version: 1.0.5".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `chinoscriba-1.0.4/chinoscriba/models/__init__.py` & `chinoscriba-1.0.5/chinoscriba/models/__init__.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/models/audit_log.py` & `chinoscriba-1.0.5/chinoscriba/models/audit_log.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/models/block.py` & `chinoscriba-1.0.5/chinoscriba/models/block.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/models/event.py` & `chinoscriba-1.0.5/chinoscriba/models/event.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/models/inline_response200.py` & `chinoscriba-1.0.5/chinoscriba/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/models/inline_response2001.py` & `chinoscriba-1.0.5/chinoscriba/models/inline_response2001.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/models/inline_response2002.py` & `chinoscriba-1.0.5/chinoscriba/models/inline_response2002.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/models/inline_response200_bis.py` & `chinoscriba-1.0.5/chinoscriba/models/inline_response200_bis.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/models/log.py` & `chinoscriba-1.0.5/chinoscriba/models/log.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/models/multi_audit_log_serializer_output.py` & `chinoscriba-1.0.5/chinoscriba/models/multi_audit_log_serializer_output.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/models/search_request.py` & `chinoscriba-1.0.5/chinoscriba/models/search_request.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/models/sort_rule.py` & `chinoscriba-1.0.5/chinoscriba/models/sort_rule.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/models/stat.py` & `chinoscriba-1.0.5/chinoscriba/models/stat.py`

 * *Files identical despite different names*

### Comparing `chinoscriba-1.0.4/chinoscriba/rest.py` & `chinoscriba-1.0.5/chinoscriba/rest.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,17 @@
     Chino.io :: Scriba API
 
     An API to create and search immutable, legally-validated Audit Logs.<br>Provided by Chino.io - https://www.chino.io  # noqa: E501
 
     OpenAPI spec version: v1
     Contact: tech-support@chino.io
     Generated by: https://github.com/swagger-api/swagger-codegen.git
+
+    Updated by Andrea on 2023/04/19 to add a workaround for
+    https://github.com/swagger-api/swagger-codegen/issues/2305 (see line 220)
 """
 
 from __future__ import absolute_import
 
 import io
 import json
 import logging
@@ -211,18 +214,27 @@
         except urllib3.exceptions.SSLError as e:
             msg = "{0}\n{1}".format(type(e).__name__, str(e))
             raise ApiException(status=0, reason=msg)
 
         if _preload_content:
             r = RESTResponse(r)
 
-            # In the python 3, the response.data is bytes.
-            # we need to decode it to string.
-            if six.PY3:
-                r.data = r.data.decode('utf8')
+            # Use try/except to handle issue:
+            # https://github.com/swagger-api/swagger-codegen/issues/2305
+            try:
+                # In the python 3, the response.data is bytes.
+                # we need to decode it to string.
+                if six.PY3:
+                    r.data = r.data.decode('utf8')
+            except UnicodeDecodeError:
+                content_type = r.getheader("Content-Type", None)
+                if 'application/zip' in content_type:
+                    pass  # allow zip content to be passed as bytes
+                else:
+                    raise
 
             # log response body
             logger.debug("response body: %s", r.data)
 
         if not 200 <= r.status <= 299:
             raise ApiException(http_resp=r)
```

### Comparing `chinoscriba-1.0.4/chinoscriba.egg-info/SOURCES.txt` & `chinoscriba-1.0.5/chinoscriba.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,8 +24,9 @@
 chinoscriba/models/inline_response200_bis.py
 chinoscriba/models/log.py
 chinoscriba/models/multi_audit_log_serializer_output.py
 chinoscriba/models/search_request.py
 chinoscriba/models/sort_rule.py
 chinoscriba/models/stat.py
 test/__init__.py
-test/test_default_api.py
+test/test_default_api.py
+test/utils.py
```

### Comparing `chinoscriba-1.0.4/setup.py` & `chinoscriba-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 NAME = "chinoscriba"
-VERSION = "1.0.4"
+VERSION = "1.0.5"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `chinoscriba-1.0.4/test/test_default_api.py` & `chinoscriba-1.0.5/test/test_default_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,27 +11,34 @@
     Implemented by: Andrea Arighi <andrea@chino.io>
                     Daniele Zanotelli <daniele@chino.io>
 
 """
 
 from __future__ import absolute_import
 
+import datetime
 import io
 import os
 import time
 import unittest
 import zipfile
+from unittest.mock import patch
 
 from chinoscriba import Configuration, ApiClient, AuditLog
 from chinoscriba import BlocksApi, EventsApi, LogsApi, StatsApi
 from chinoscriba.rest import ApiException
+from dateutil.tz import tzutc
+from django.utils import timezone
 
-# # SDK Configuration
 from nose.plugins.attrib import attr
 
+from .utils import _mock_nullable_stats
+
+
+# # SDK Configuration
 host = os.environ.get('host', "http://localhost:8000")
 # Basic auth
 configuration = Configuration()
 configuration.host = host
 configuration.username = os.environ.get(
     'customer_id', "NO AUTH (set the env variable 'customer_id')")
 configuration.password = os.environ.get(
@@ -481,14 +488,34 @@
         with self.assertRaises(ApiException):
             self.api.stats_read(t=10)
         with self.assertRaises(ApiException):
                 self.api.stats_read(t=None)
         with self.assertRaises(ApiException):
             self.api.stats_read(t="")
 
+    @patch('chinoscriba.ApiClient.request', new_callable=_mock_nullable_stats)
+    def test_nullable_items(self, mock_function):
+        response = self.api.stats_read()
+        print(response)
+        # assert mock_function.called
+
+        # fixme: restore when the SDK generator supports nullable fields
+        # for nullable_field in ['manual_logs', 'all_logs', 'oldest_log',
+        #                        'oldest_block']:
+        #     value = getattr(response, nullable_field, "NOT SET")
+        #     self.assertIsNone(value, msg=f"'{nullable_field}' should be None")
+
+        # ...and remove the code below
+        self.assertEquals(0, response.manual_logs)
+        self.assertEquals(0, response.all_logs)
+        # using 2001 because that's how it gets deserialized by the SDK
+        self.assertEquals(datetime.datetime(2001, 1, 1, 0, 0, tzinfo=tzutc()),
+                          response.oldest_log)
+        self.assertEquals(datetime.datetime(2001, 1, 1, 0, 0, tzinfo=tzutc()),
+                          response.oldest_block)
 
     def _verify_stats(self, stats):
         """The stats object in its dict() format
         """
         # check structure of serialized object
         stats_keys = {
             "manual_logs", "all_logs", "oldest_log", "total_blocks",
```


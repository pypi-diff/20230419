# Comparing `tmp/etsy3py-0.0.1.tar.gz` & `tmp/etsy3py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etsy3py-0.0.1.tar", last modified: Wed Apr 19 08:48:41 2023, max compression
+gzip compressed data, was "etsy3py-0.0.2.tar", last modified: Wed Apr 19 12:40:24 2023, max compression
```

## Comparing `etsy3py-0.0.1.tar` & `etsy3py-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-19 08:48:41.610989 etsy3py-0.0.1/
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)     1055 2023-04-12 13:00:44.000000 etsy3py-0.0.1/LICENSE.txt
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)      314 2023-04-19 08:48:41.610663 etsy3py-0.0.1/PKG-INFO
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)     2101 2023-04-19 08:48:24.000000 etsy3py-0.0.1/README.md
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)       38 2023-04-19 08:48:41.611105 etsy3py-0.0.1/setup.cfg
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)      478 2023-04-19 08:48:24.000000 etsy3py-0.0.1/setup.py
-drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-19 08:48:41.604894 etsy3py-0.0.1/src/
-drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-19 08:48:41.607765 etsy3py-0.0.1/src/etsy3py/
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)        0 2023-04-12 12:44:41.000000 etsy3py-0.0.1/src/etsy3py/__init__.py
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)     2278 2023-04-19 08:48:18.000000 etsy3py-0.0.1/src/etsy3py/base_client.py
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)     3205 2023-04-19 08:48:24.000000 etsy3py-0.0.1/src/etsy3py/oauth.py
-drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-19 08:48:41.610242 etsy3py-0.0.1/src/etsy3py.egg-info/
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)      314 2023-04-19 08:48:41.000000 etsy3py-0.0.1/src/etsy3py.egg-info/PKG-INFO
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)      276 2023-04-19 08:48:41.000000 etsy3py-0.0.1/src/etsy3py.egg-info/SOURCES.txt
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)        1 2023-04-19 08:48:41.000000 etsy3py-0.0.1/src/etsy3py.egg-info/dependency_links.txt
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)       32 2023-04-19 08:48:41.000000 etsy3py-0.0.1/src/etsy3py.egg-info/requires.txt
--rw-r--r--   0 sashaal-sayed   (501) staff       (20)        8 2023-04-19 08:48:41.000000 etsy3py-0.0.1/src/etsy3py.egg-info/top_level.txt
+drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-19 12:40:24.821848 etsy3py-0.0.2/
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)     1055 2023-04-12 13:00:44.000000 etsy3py-0.0.2/LICENSE.txt
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)     3644 2023-04-19 12:40:24.821504 etsy3py-0.0.2/PKG-INFO
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)     3120 2023-04-19 12:40:19.000000 etsy3py-0.0.2/README.md
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)       38 2023-04-19 12:40:24.821986 etsy3py-0.0.2/setup.cfg
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)      890 2023-04-19 12:40:19.000000 etsy3py-0.0.2/setup.py
+drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-19 12:40:24.815199 etsy3py-0.0.2/src/
+drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-19 12:40:24.818872 etsy3py-0.0.2/src/etsy3py/
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)        0 2023-04-12 12:44:41.000000 etsy3py-0.0.2/src/etsy3py/__init__.py
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)     2493 2023-04-19 12:40:19.000000 etsy3py-0.0.2/src/etsy3py/base_client.py
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)     3205 2023-04-19 08:48:24.000000 etsy3py-0.0.2/src/etsy3py/oauth.py
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)    15320 2023-04-19 12:40:19.000000 etsy3py-0.0.2/src/etsy3py/v3.py
+drwxr-xr-x   0 sashaal-sayed   (501) staff       (20)        0 2023-04-19 12:40:24.821056 etsy3py-0.0.2/src/etsy3py.egg-info/
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)     3644 2023-04-19 12:40:24.000000 etsy3py-0.0.2/src/etsy3py.egg-info/PKG-INFO
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)      294 2023-04-19 12:40:24.000000 etsy3py-0.0.2/src/etsy3py.egg-info/SOURCES.txt
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)        1 2023-04-19 12:40:24.000000 etsy3py-0.0.2/src/etsy3py.egg-info/dependency_links.txt
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)       32 2023-04-19 12:40:24.000000 etsy3py-0.0.2/src/etsy3py.egg-info/requires.txt
+-rw-r--r--   0 sashaal-sayed   (501) staff       (20)        8 2023-04-19 12:40:24.000000 etsy3py-0.0.2/src/etsy3py.egg-info/top_level.txt
```

### Comparing `etsy3py-0.0.1/LICENSE.txt` & `etsy3py-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etsy3py-0.0.1/README.md` & `etsy3py-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,128 @@
+Metadata-Version: 2.1
+Name: etsy3py
+Version: 0.0.2
+Summary: ETSY API v3 Client
+Home-page: https://github.com/damhuman/Etsy3Py
+Author: Anton Dasyuk, Ali-Abdulla
+Author-email: anton.dasyuk@gmail.com, alexukr1999@gmail.com
+License: MIT
+Keywords: etsy,api,client,etsy v3 api
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 # Etsy3Py
 Client for Etsy API v3
 
 ## Installation
 You can install etsy3py using pip:
 
-`pip install etsy3py`
+``` python
+pip install etsy3py
+```
 
 
 # Authentication step-by-step
 `EtsyOAuthClient` is a Python class that provides an authentication client for the Etsy marketplace API, 
 allowing users to connect to the API using OAuth2 authentication.
 
 ## Usage
 Here is an example of how to use the EtsyOAuthClient to obtain an access token from the Etsy API.
 
-`from etsy3py.oauth import EtsyOAuthClient`
+``` python
+from etsy3py.oauth import EtsyOAuthClient
+```
 
 Replace these with your own values from the Etsy Developer Console
 
-`client_id = 'your_client_id'
+``` python
+client_id = 'your_client_id'
 client_secret = 'your_client_secret'
 redirect_uri = 'your_redirect_uri' 
-scope = ['your_scope_1', 'your_scope_2', ...]`
+scope = ['your_scope_1', 'your_scope_2', ...]
+```
 
 Create an instance of the EtsyOAuthClient
 
-`client = EtsyOAuthClient(client_id, client_secret, redirect_uri, scope)`
+``` python
+client = EtsyOAuthClient(client_id, client_secret, redirect_uri, scope)
+```
 
 Get the authorization URL
 
-`authorization_url, state = client.authorization_url()`
+``` python
+authorization_url, state = client.authorization_url()
+```
 
 Redirect the user to the authorization URL to grant access. Once the user has granted access, get the authorization code and use it to obtain an access token
 
-`authorization_code = 'the_authorization_code'
-access_token = client.fetch_token(authorization_code)`
+``` python
+authorization_code = 'the_authorization_code'
+access_token = client.fetch_token(authorization_code)
+```
 
 You can now use the access token to make requests to the Etsy API
 
 ## Refresh token
 
 The `refresh_token` method of the `EtsyOAuthClient` class requests a new access token from the authorization server using a refresh token.
 
-**Parameters**
+### Parameters
 
 `refresh_token` (required): The refresh token used to obtain a new access token.
 
-**Return Value**
+### Return Value
 
 The `refresh_token` method returns a dictionary containing the new access token and any additional data returned by the authorization server.
 
-**Example**
+### Example
 
 Replace these with your own values from the Etsy Developer Console
 
-`client_id = 'your_client_id'
-client_secret = 'your_client_secret'`
+``` python
+client_id = 'your_client_id'
+client_secret = 'your_client_secret'
 
-Create an instance of the EtsyOAuthClient
+# create an instance of the EtsyOAuthClient
+
+client = EtsyOAuthClient(client_id, client_secret)
+
+# if the access token expires, you can use the refresh token to obtain a new access token and additional data 
+
+new_access_token = client.refresh_token(refresh_token)
+```
+
+# Etsy API
+This is a Python client for the Etsy API. 
+The client makes it easy to interact with the Etsy API and perform operations on a user's behalf.
+
+### Requirements
+Python 3.6 or higher
+
+## Usage
+To use the EtsyApi class, you will need to obtain an access token from the Etsy API.
+
+``` python
+from etsy3py.v3 import EtsyApi
+
+access_token = "YOUR_ACCESS_TOKEN"
+client_id = "YOUR_CLIENT_ID"
 
-`client = EtsyOAuthClient(client_id, client_secret)`
+etsy_api = EtsyApi(access_token=access_token, client_id=client_id)
+# you can then call methods on the etsy_api object to interact with the Etsy API.
+```
 
-If the access token expires, you can use the refresh token to obtain a new access token and additional data 
+### Authentication
+The EtsyApi class uses OAuth 2.0 authentication. You will need to obtain an access token from the Etsy API 
+before using the client. You can obtain an access token by following the
+instructions in the Etsy API documentation.
 
-`new_access_token = client.refresh_token(refresh_token)`
+### Rate Limiting
+The Etsy API has a rate limiting policy that limits the number of requests that can be made in a given time period.
 
+#### This package is licensed under the MIT License.
 
-#### This package is licensed under the MIT License.
```

### Comparing `etsy3py-0.0.1/src/etsy3py/base_client.py` & `etsy3py-0.0.2/src/etsy3py/base_client.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,63 @@
+from typing import Type
+
+import requests
 from requests.auth import HTTPBasicAuth
 from requests import Request, Session
- 
- 
+
+
 class BaseApiClient:
     base_url = "https://openapi.etsy.com"
     __token_type = None
     __token = None
-    __token_expire = None
+    __client_id = None
     session = Session()
  
     def _make_request(self,
                       path: str,
                       custom_base: str = None,
                       method: str = 'GET',
                       headers: dict = None,
                       data: dict = None,
                       params: dict = None,
-                      auth_type: str = 'token'):
-        if auth_type == 'token':
-            self.check_token()
+                      auth_type: str = 'token') -> Type[requests.Response]:
+
         if not headers:
             headers = {}
  
         request_url = f"{custom_base if custom_base else self.base_url}{path}"
  
         auth = None
         if auth_type == 'basic':
             auth = HTTPBasicAuth(1, 1)
         if auth_type == 'token':
             headers['Authorization'] = f'{self.__token_type} {self.__token}'
+            headers['x-api-key'] = f'{self.__client_id}'
  
         request = Request(method=method,
                           url=request_url,
                           headers=headers,
                           data=data,
                           params=params,
                           auth=auth).prepare()
         response = self.session.send(request)
         return response
  
-    def _post(self, path: str, data: dict = None, headers: dict = None, auth_type: str = 'none'):
+    def _post(self, path: str, data: dict = None, headers: dict = None,
+              auth_type: str = 'none') -> Type[requests.Response]:
         return self._make_request(path=path, method='POST', data=data,
                                   headers=headers, auth_type=auth_type)
  
-    def _get(self, path: str, params: dict = None, headers: dict = None, auth_type: str = 'none'):
+    def _get(self, path: str, params: dict = None, headers: dict = None,
+             auth_type: str = 'none') -> Type[requests.Response]:
         return self._make_request(path=path, method='GET', params=params,
                                   headers=headers, auth_type=auth_type)
 
-    def _put(self, path: str, params: dict = None, headers: dict = None, auth_type: str = 'none'):
-        return self._make_request(path=path, method='PUT', params=params,
+    def _put(self, path: str, data: dict = None, headers: dict = None,
+             auth_type: str = 'none') -> Type[requests.Response]:
+        return self._make_request(path=path, method='PUT', data=data,
                                   headers=headers, auth_type=auth_type)
 
-    def _delete(self, path: str, params: dict = None, headers: dict = None, auth_type: str = 'none'):
+    def _delete(self, path: str, params: dict = None, headers: dict = None,
+                auth_type: str = 'none') -> Type[requests.Response]:
         return self._make_request(path=path, method='DELETE', params=params,
                                   headers=headers, auth_type=auth_type)
```

### Comparing `etsy3py-0.0.1/src/etsy3py/oauth.py` & `etsy3py-0.0.2/src/etsy3py/oauth.py`

 * *Files identical despite different names*


# Comparing `tmp/crosslab_api_client-0.2.1.tar.gz` & `tmp/crosslab_api_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslab_api_client-0.2.1.tar", last modified: Tue Feb 21 23:49:28 2023, max compression
+gzip compressed data, was "crosslab_api_client-0.2.2.tar", last modified: Wed Apr 19 18:27:18 2023, max compression
```

## Comparing `crosslab_api_client-0.2.1.tar` & `crosslab_api_client-0.2.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:49:28.190063 crosslab_api_client-0.2.1/
--rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-02-21 23:49:28.190063 crosslab_api_client-0.2.1/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:33:01.000000 crosslab_api_client-0.2.1/README.md
--rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.1/pyproject.toml
--rw-r--r--   0 dev       (1000) docker-host   (967)      605 2023-02-21 23:49:28.190063 crosslab_api_client-0.2.1/setup.cfg
--rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.1/setup.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:49:28.190063 crosslab_api_client-0.2.1/src/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:49:28.190063 crosslab_api_client-0.2.1/src/crosslab/
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:49:28.190063 crosslab_api_client-0.2.1/src/crosslab/api_client/
--rw-r--r--   0 dev       (1000) docker-host   (967)       49 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.1/src/crosslab/api_client/__init__.py
--rw-r--r--   0 dev       (1000) docker-host   (967)    57960 2023-02-21 23:49:21.000000 crosslab_api_client-0.2.1/src/crosslab/api_client/client.py
--rw-r--r--   0 dev       (1000) docker-host   (967)       50 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.1/src/crosslab/api_client/exceptions.py
--rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.1/src/crosslab/api_client/py.typed
--rw-r--r--   0 dev       (1000) docker-host   (967)   767195 2023-02-21 23:49:21.000000 crosslab_api_client-0.2.1/src/crosslab/api_client/schemas.py
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:49:28.190063 crosslab_api_client-0.2.1/src/crosslab_api_client.egg-info/
--rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-02-21 23:49:28.000000 crosslab_api_client-0.2.1/src/crosslab_api_client.egg-info/PKG-INFO
--rw-r--r--   0 dev       (1000) docker-host   (967)      475 2023-02-21 23:49:28.000000 crosslab_api_client-0.2.1/src/crosslab_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-02-21 23:49:28.000000 crosslab_api_client-0.2.1/src/crosslab_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)       24 2023-02-21 23:49:28.000000 crosslab_api_client-0.2.1/src/crosslab_api_client.egg-info/requires.txt
--rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-02-21 23:49:28.000000 crosslab_api_client-0.2.1/src/crosslab_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-02-21 23:49:28.190063 crosslab_api_client-0.2.1/tests/
--rw-r--r--   0 dev       (1000) docker-host   (967)   471144 2023-02-21 23:49:25.000000 crosslab_api_client-0.2.1/tests/test_openapi.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:27:18.488827 crosslab_api_client-0.2.2/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-04-19 18:27:18.488827 crosslab_api_client-0.2.2/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:06:55.000000 crosslab_api_client-0.2.2/README.md
+-rw-r--r--   0 dev       (1000) docker-host   (967)       87 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.2/pyproject.toml
+-rw-r--r--   0 dev       (1000) docker-host   (967)      624 2023-04-19 18:27:18.488827 crosslab_api_client-0.2.2/setup.cfg
+-rw-r--r--   0 dev       (1000) docker-host   (967)       37 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.2/setup.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:27:18.485494 crosslab_api_client-0.2.2/src/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:27:18.485494 crosslab_api_client-0.2.2/src/crosslab/
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:27:18.485494 crosslab_api_client-0.2.2/src/crosslab/api_client/
+-rw-r--r--   0 dev       (1000) docker-host   (967)       58 2023-04-03 16:08:17.000000 crosslab_api_client-0.2.2/src/crosslab/api_client/__init__.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)    56595 2023-04-19 18:27:11.000000 crosslab_api_client-0.2.2/src/crosslab/api_client/client.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)       50 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.2/src/crosslab/api_client/exceptions.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)      804 2023-04-03 16:08:17.000000 crosslab_api_client-0.2.2/src/crosslab/api_client/improved_client.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)        0 2023-02-10 09:58:35.000000 crosslab_api_client-0.2.2/src/crosslab/api_client/py.typed
+-rw-r--r--   0 dev       (1000) docker-host   (967)    73241 2023-04-19 18:27:11.000000 crosslab_api_client-0.2.2/src/crosslab/api_client/schemas.py
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:27:18.485494 crosslab_api_client-0.2.2/src/crosslab_api_client.egg-info/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      331 2023-04-19 18:27:18.000000 crosslab_api_client-0.2.2/src/crosslab_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 dev       (1000) docker-host   (967)      548 2023-04-19 18:27:18.000000 crosslab_api_client-0.2.2/src/crosslab_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        1 2023-04-19 18:27:18.000000 crosslab_api_client-0.2.2/src/crosslab_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)       42 2023-04-19 18:27:18.000000 crosslab_api_client-0.2.2/src/crosslab_api_client.egg-info/requires.txt
+-rw-r--r--   0 dev       (1000) docker-host   (967)        9 2023-04-19 18:27:18.000000 crosslab_api_client-0.2.2/src/crosslab_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 dev       (1000) docker-host   (967)        0 2023-04-19 18:27:18.488827 crosslab_api_client-0.2.2/tests/
+-rw-r--r--   0 dev       (1000) docker-host   (967)      722 2023-04-03 16:08:17.000000 crosslab_api_client-0.2.2/tests/test_improved_client.py
+-rw-r--r--   0 dev       (1000) docker-host   (967)   463687 2023-04-19 18:27:15.000000 crosslab_api_client-0.2.2/tests/test_openapi.py
```

### Comparing `crosslab_api_client-0.2.1/setup.cfg` & `crosslab_api_client-0.2.2/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = crosslab_api_client
-version = 0.2.1
+version = 0.2.2
 author = Johannes Nau
 author_email = johannes.nau@tu-ilmenau.de
 description = The CrossLab API Client
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: Other/Proprietary License
 	Operating System :: OS Independent
@@ -14,14 +14,15 @@
 	= src
 packages = find_namespace:
 python_requires = >=3.8, <3.12
 include_package_data = True
 install_requires = 
 	aiohttp
 	python-dateutil
+	typing_extensions
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 * = py.typed
```

### Comparing `crosslab_api_client-0.2.1/src/crosslab/api_client/client.py` & `crosslab_api_client-0.2.2/src/crosslab/api_client/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,120 @@
 import aiohttp
 import re
 from typing import Optional, Any, Dict, List, Tuple, Union
-from crosslab.api_client.schemas import *  # noqa: F403
 from crosslab.api_client.exceptions import AuthorizationException
 
+from crosslab.api_client.schemas import (
+    LoginRequest,
+    LoginResponse,
+    LogoutRequest,
+    LogoutResponse,
+    CreateDeviceAuthenticationTokenResponse,
+    ListUsersResponse,
+    CreateUserRequest,
+    CreateUserResponse,
+    GetUserResponse,
+    UpdateUserRequest,
+    UpdateUserResponse,
+    DeleteUserResponse,
+    GetRolesOfUserResponse,
+    AddRolesToUserRequest,
+    AddRolesToUserResponse,
+    RemoveRolesFromUserRequest,
+    RemoveRolesFromUserResponse,
+    ListRolesResponse,
+    CreateRoleRequest,
+    CreateRoleResponse,
+    GetRoleResponse,
+    UpdateRoleRequest,
+    UpdateRoleResponse,
+    DeleteRoleResponse,
+    GetUsersWithRoleResponse,
+    AddUsersToRoleRequest,
+    AddUsersToRoleResponse,
+    RemoveUsersFromRoleRequest,
+    RemoveUsersFromRoleResponse,
+    GetIdentityResponse,
+    UpdateIdentityRequest,
+    UpdateIdentityResponse,
+    GetScheduleRequest,
+    GetScheduleResponse,
+    BookExperimentRequest,
+    BookExperimentResponse,
+    UpdateBookingRequest,
+    UpdateBookingResponse,
+    CancelBookingResponse,
+    GetBookingResponse,
+    DeleteBookingResponse,
+    LockBookingResponse,
+    UnlockBookingResponse,
+    ListDevicesResponse,
+    CreateDeviceRequest,
+    CreateDeviceResponse,
+    GetDeviceResponse,
+    UpdateDeviceRequest,
+    UpdateDeviceResponse,
+    DeleteDeviceResponse,
+    InstantiateDeviceResponse,
+    AddAvailabilityRulesRequest,
+    AddAvailabilityRulesResponse,
+    CreateWebsocketTokenResponse,
+    SendSignalingMessageRequest,
+    SendSignalingMessageResponse,
+    ListPeerconnectionsResponse,
+    CreatePeerconnectionRequest,
+    CreatePeerconnectionResponse,
+    GetPeerconnectionResponse,
+    DeletePeerconnectionResponse,
+    ListExperimentsResponse,
+    CreateExperimentRequest,
+    CreateExperimentResponse,
+    GetExperimentResponse,
+    UpdateExperimentRequest,
+    UpdateExperimentResponse,
+    DeleteExperimentResponse,
+    ListInstitutionsResponse,
+    CreateInstitutionRequest,
+    CreateInstitutionResponse,
+    GetInstitutionResponse,
+    UpdateInstitutionRequest,
+    UpdateInstitutionResponse,
+    DeleteInstitutionResponse,
+    ListUpdatesResponse,
+    CreateUpdateRequest,
+    CreateUpdateResponse,
+    GetUpdateResponse,
+    PatchUpdateRequest,
+    PatchUpdateResponse,
+    DeleteUpdateResponse
+)
+
 
 class APIClient:
     BASE_URL: Optional[str] = None
     authToken: Optional[str] = None
 
     def __init__(self, base_url: Optional[str] = None, authToken: Optional[str] = None):
         if base_url is None:
             base_url = self.BASE_URL
         elif base_url.endswith('/'):
             base_url = base_url[:-1]
         self.BASE_URL = base_url
         self.authToken = authToken
 
-    def set_auth_token(self, authToken: str):
+    def set_auth_token(self, authToken: Optional[str]):
         self.authToken = authToken
         if self.http_session is not None:
-            self.http_session.headers.update({"Authorization": f'Bearer {authToken}'})
+            if authToken is not None:
+                self.http_session.headers.update(
+                    {"Authorization": f"Bearer {authToken}"}
+                )
+            else:
+                if "Authorization" in self.http_session.headers:
+                    del self.http_session.headers["Authorization"]
 
     async def __aenter__(self):
         self.http_session = aiohttp.ClientSession()
         if self.authToken is not None:
             self.http_session.headers.update({"Authorization": f'Bearer {self.authToken}'})
         return self
 
@@ -69,69 +159,61 @@
                 return resp.status, await resp.text()
             else:
                 try:
                     return resp.status, await resp.json()
                 except aiohttp.ContentTypeError:
                     return resp.status, await resp.text()
 
-    async def login(self, body: PostLoginRequestBodyWrite, url: str = "/login"):  # noqa: E501
+    async def login(self, body: LoginRequest, url: str = "/login") -> LoginResponse:  # noqa: E501
         """
         Login user
         
         This endpoint will login a user and return an access token for the use of the microservice architecture."""  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(login)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/login'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = post_login_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="post", body=body)
            
         # transform response
         if status == 201:
-            return post_login_response_body201_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def logout(self, body: PostLogoutRequestBodyWrite, url: str = "/logout"):  # noqa: E501
+    async def logout(self, body: LogoutRequest, url: str = "/logout") -> LogoutResponse:  # noqa: E501
         """
         Logout user
         
         This endpoint will logout a user and remove the corresponding access token for the use of the microservice architecture."""  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(logout)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/logout'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = post_logout_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="post", body=body)
            
         # transform response
         if status == 204:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def create_device_authentication_token(self, device_url: str, url: str = "/device_authentication_token"):  # noqa: E501
+    async def create_device_authentication_token(self, device_url: str, url: str = "/device_authentication_token") -> CreateDeviceAuthenticationTokenResponse:  # noqa: E501
         """
         Create a device authentication token
         
         This endpoint will create a new device authentication token."""  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
@@ -146,713 +228,649 @@
         # build query params
         query_params: Dict[str, Union[List[str], str]] = {}
         if device_url:
             if isinstance(device_url, list):
                 query_params['device_url'] = device_url
             else:
                 query_params['device_url'] = str(device_url)
+        
         # make http call
         status, resp = await self._fetch(valid_url, method="post", params=query_params)
            
         # transform response
         if status == 201:
-            return post_device_authentication_token_response_body201_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def list_users(self, url: str = "/users"):  # noqa: E501
+    async def list_users(self, url: str = "/users") -> ListUsersResponse:  # noqa: E501
         """
         Get all users
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(users)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/users'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_users_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def create_user(self, body: PostUsersRequestBodyWrite, url: str = "/users"):  # noqa: E501
+    async def create_user(self, body: CreateUserRequest, url: str = "/users") -> CreateUserResponse:  # noqa: E501
         """
         Create a user
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(users)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/users'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = post_users_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="post", body=body)
            
         # transform response
         if status == 201:
-            return post_users_response_body201_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def get_user(self, url: str):  # noqa: E501
+    async def get_user(self, url: str) -> GetUserResponse:  # noqa: E501
         """
         Get a user
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(users\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_user_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def update_user(self, url: str, body: Optional[PatchUserRequestBodyWrite] = None):  # noqa: E501
+    async def update_user(self, url: str, body: Optional[UpdateUserRequest] = None) -> UpdateUserResponse:  # noqa: E501
         """
         Update a user
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(users\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = patch_user_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="patch", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="patch", body=body)
            
         # transform response
         if status == 200:
-            return patch_user_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def delete_user(self, url: str):  # noqa: E501
+    async def delete_user(self, url: str) -> DeleteUserResponse:  # noqa: E501
         """
         Delete a user
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(users\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="delete")
            
         # transform response
         if status == 204:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def get_roles_of_user(self, url: str):  # noqa: E501
+    async def get_roles_of_user(self, url: str) -> GetRolesOfUserResponse:  # noqa: E501
         """
         Get roles of user
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(users\/[^?]*?)(\/roles)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/roles'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_user_roles_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def add_roles_to_user(self, url: str, body: Optional[List[str]] = None):  # noqa: E501
+    async def add_roles_to_user(self, url: str, body: Optional[AddRolesToUserRequest] = None) -> AddRolesToUserResponse:  # noqa: E501
         """
         Add roles to user
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(users\/[^?]*?)(\/roles)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/roles'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = post_user_roles_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="post", body=body)
            
         # transform response
         if status == 204:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def remove_roles_from_user(self, url: str, body: Optional[List[str]] = None):  # noqa: E501
+    async def remove_roles_from_user(self, url: str, body: Optional[RemoveRolesFromUserRequest] = None) -> RemoveRolesFromUserResponse:  # noqa: E501
         """
         Remove roles from user
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(users\/[^?]*?)(\/roles)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/roles'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = delete_user_roles_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="delete", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="delete", body=body)
            
         # transform response
         if status == 204:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def list_roles(self, url: str = "/roles"):  # noqa: E501
+    async def list_roles(self, url: str = "/roles") -> ListRolesResponse:  # noqa: E501
         """
         Get all roles
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(roles)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/roles'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_roles_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def create_role(self, body: Optional[PostRolesRequestBodyWrite] = None, url: str = "/roles"):  # noqa: E501
+    async def create_role(self, url: str = "/roles", body: Optional[CreateRoleRequest] = None) -> CreateRoleResponse:  # noqa: E501
         """
         Create a role
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(roles)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/roles'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = post_roles_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="post", body=body)
            
         # transform response
         if status == 201:
-            return post_roles_response_body201_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def get_role(self, url: str):  # noqa: E501
+    async def get_role(self, url: str) -> GetRoleResponse:  # noqa: E501
         """
         Get a role
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(roles\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_role_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def update_role(self, url: str, body: Optional[PatchRoleRequestBodyWrite] = None):  # noqa: E501
+    async def update_role(self, url: str, body: Optional[UpdateRoleRequest] = None) -> UpdateRoleResponse:  # noqa: E501
         """
         Update a role
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(roles\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = patch_role_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="patch", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="patch", body=body)
            
         # transform response
         if status == 200:
-            return patch_role_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def delete_role(self, url: str):  # noqa: E501
+    async def delete_role(self, url: str) -> DeleteRoleResponse:  # noqa: E501
         """
         Delete a role
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(roles\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="delete")
            
         # transform response
         if status == 204:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def get_users_with_role(self, url: str):  # noqa: E501
+    async def get_users_with_role(self, url: str) -> GetUsersWithRoleResponse:  # noqa: E501
         """
         Get users with role
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(roles\/[^?]*?)(\/users)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/users'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_role_users_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def add_users_to_role(self, url: str, body: Optional[List[str]] = None):  # noqa: E501
+    async def add_users_to_role(self, url: str, body: Optional[AddUsersToRoleRequest] = None) -> AddUsersToRoleResponse:  # noqa: E501
         """
         Add users to role
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(roles\/[^?]*?)(\/users)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/users'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = post_role_users_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="post", body=body)
            
         # transform response
         if status == 204:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def remove_users_from_role(self, url: str, body: Optional[List[str]] = None):  # noqa: E501
+    async def remove_users_from_role(self, url: str, body: Optional[RemoveUsersFromRoleRequest] = None) -> RemoveUsersFromRoleResponse:  # noqa: E501
         """
         Remove users from role
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(roles\/[^?]*?)(\/users)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/users'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = delete_role_users_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="delete", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="delete", body=body)
            
         # transform response
         if status == 204:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def get_identity(self, url: str = "/identity"):  # noqa: E501
+    async def get_identity(self, url: str = "/identity") -> GetIdentityResponse:  # noqa: E501
         """
         Get identity
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(identity)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/identity'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_identity_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def update_identity(self, body: Optional[PatchIdentityRequestBodyWrite] = None, url: str = "/identity"):  # noqa: E501
+    async def update_identity(self, url: str = "/identity", body: Optional[UpdateIdentityRequest] = None) -> UpdateIdentityResponse:  # noqa: E501
         """
         Update identity
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(identity)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/identity'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = patch_identity_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="patch", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="patch", body=body)
            
         # transform response
         if status == 200:
-            return patch_identity_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def get_schedule(self, body: Optional[PostScheduleRequestBodyWrite] = None, url: str = "/schedule"):  # noqa: E501
+    async def get_schedule(self, url: str = "/schedule", body: Optional[GetScheduleRequest] = None) -> GetScheduleResponse:  # noqa: E501
         """
         Returns the free / booked times for given experiment.
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(schedule)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/schedule'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = post_schedule_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="post", body=body)
            
         # transform response
         if status == 200:
-            return post_schedule_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def book_experiment(self, body: Optional[PostBookingRequestBodyWrite] = None, url: str = "/booking"):  # noqa: E501
+    async def book_experiment(self, url: str = "/booking", body: Optional[BookExperimentRequest] = None) -> BookExperimentResponse:  # noqa: E501
         """
         Books an experiment.
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(booking)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/booking'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = post_booking_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="post", body=body)
            
         # transform response
         if status == 200:
-            return post_booking_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def update_booking(self, url: str, body: PatchBookingRequestBodyWrite):  # noqa: E501
+    async def update_booking(self, url: str, body: UpdateBookingRequest) -> UpdateBookingResponse:  # noqa: E501
         """
         Allows the addition of devices to a booking (removing of devices is not supportet) or the registration of callbacks.
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(booking\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = patch_booking_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="patch", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="patch", body=body)
            
         # transform response
         if status == 200:
-            return patch_booking_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def cancel_booking(self, url: str):  # noqa: E501
+    async def cancel_booking(self, url: str) -> CancelBookingResponse:  # noqa: E501
         """
         Cancels a booking, as long as the booking was originally done by you.
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(booking\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="delete")
            
         # transform response
         if status == 200:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def get_booking(self, url: str):  # noqa: E501
+    async def get_booking(self, url: str) -> GetBookingResponse:  # noqa: E501
         """
         Returns whether a list of devices is currently booked for a user
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(booking\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_booking_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def delete_booking(self, url: str):  # noqa: E501
+    async def delete_booking(self, url: str) -> DeleteBookingResponse:  # noqa: E501
         """
         Allows selected persons (like lab manager) to remove a user booking. To avoid mistakes, this is a different path than normal delete.
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(booking\/[^?]*?)(\/destroy)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/destroy'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="delete")
            
         # transform response
         if status == 200:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def lock_booking(self, url: str):  # noqa: E501
+    async def lock_booking(self, url: str) -> LockBookingResponse:  # noqa: E501
         """
         Locks the current booking so the devices can be used. This sets the status to "active" This means that the booking can not be cancelled or (currently not implemented) the end time can not be set to a prior time. If called multiple times, the booking will be locked only once.
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(booking\/[^?]*?)(\/lock)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/lock'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="put")
            
         # transform response
         if status == 200:
-            return put_booking_lock_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def unlock_booking(self, url: str):  # noqa: E501
+    async def unlock_booking(self, url: str) -> UnlockBookingResponse:  # noqa: E501
         """
         Unlocks all devices belonging to a booking, status will be set to 'booked'.
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(booking\/[^?]*?)(\/lock)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/lock'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="delete")
            
         # transform response
         if status == 200:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def list_devices(self, url: str = "/devices"):  # noqa: E501
+    async def list_devices(self, url: str = "/devices") -> ListDevicesResponse:  # noqa: E501
         """
         List devices
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(devices)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/devices'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_devices_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def create_device(self, body: PostDevicesRequestBodyWrite, changedUrl: Optional[str] = None, url: str = "/devices"):  # noqa: E501
+    async def create_device(self, body: CreateDeviceRequest, url: str = "/devices", changedUrl: Optional[str] = None) -> CreateDeviceResponse:  # noqa: E501
         """
         Create a new device
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(devices)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/devices'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
 
-        # transform body
-        transformedBody = post_devices_request_body_write_to_dict(body) if body else None
-
         # build query params
         query_params: Dict[str, Union[List[str], str]] = {}
         if changedUrl:
             if isinstance(changedUrl, list):
                 query_params['changedUrl'] = changedUrl
             else:
                 query_params['changedUrl'] = str(changedUrl)
+        
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody, params=query_params)
+        status, resp = await self._fetch(valid_url, method="post", body=body, params=query_params)
            
         # transform response
         if status == 201:
-            return post_devices_response_body201_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def get_device(self, url: str, flat_group: Optional[bool] = None):  # noqa: E501
+    async def get_device(self, url: str, flat_group: Optional[bool] = None) -> GetDeviceResponse:  # noqa: E501
         """
         View a registered device
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
@@ -866,79 +884,77 @@
         # build query params
         query_params: Dict[str, Union[List[str], str]] = {}
         if flat_group:
             if isinstance(flat_group, list):
                 query_params['flat_group'] = flat_group
             else:
                 query_params['flat_group'] = str(flat_group)
+        
         # make http call
         status, resp = await self._fetch(valid_url, method="get", params=query_params)
            
         # transform response
         if status == 200:
-            return get_device_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def update_device(self, url: str, body: Optional[PatchDeviceRequestBodyWrite] = None, changedUrl: Optional[str] = None):  # noqa: E501
+    async def update_device(self, url: str, body: Optional[UpdateDeviceRequest] = None, changedUrl: Optional[str] = None) -> UpdateDeviceResponse:  # noqa: E501
         """
         Update an existing device
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(devices\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
 
-        # transform body
-        transformedBody = patch_device_request_body_write_to_dict(body) if body else None
-
         # build query params
         query_params: Dict[str, Union[List[str], str]] = {}
         if changedUrl:
             if isinstance(changedUrl, list):
                 query_params['changedUrl'] = changedUrl
             else:
                 query_params['changedUrl'] = str(changedUrl)
+        
         # make http call
-        status, resp = await self._fetch(valid_url, method="patch", body=transformedBody, params=query_params)
+        status, resp = await self._fetch(valid_url, method="patch", body=body, params=query_params)
            
         # transform response
         if status == 200:
-            return patch_device_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def delete_device(self, url: str):  # noqa: E501
+    async def delete_device(self, url: str) -> DeleteDeviceResponse:  # noqa: E501
         """
         Delete a registered device
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(devices\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="delete")
            
         # transform response
         if status == 204:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def instantiate_device(self, url: str, changedUrl: Optional[str] = None):  # noqa: E501
+    async def instantiate_device(self, url: str, changedUrl: Optional[str] = None) -> InstantiateDeviceResponse:  # noqa: E501
         """
         Instantiate a cloud instantiable device
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
@@ -952,288 +968,271 @@
         # build query params
         query_params: Dict[str, Union[List[str], str]] = {}
         if changedUrl:
             if isinstance(changedUrl, list):
                 query_params['changedUrl'] = changedUrl
             else:
                 query_params['changedUrl'] = str(changedUrl)
+        
         # make http call
         status, resp = await self._fetch(valid_url, method="post", params=query_params)
            
         # transform response
         if status == 201:
-            return post_device_response_body201_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def add_availability_rules(self, url: str, body: Optional[List[FluffyAvailabilityRule]] = None):  # noqa: E501
+    async def add_availability_rules(self, url: str, body: Optional[AddAvailabilityRulesRequest] = None) -> AddAvailabilityRulesResponse:  # noqa: E501
         """
         Update the device availability
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(devices\/[^?]*?)(\/availability)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/availability'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = post_device_availability_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="post", body=body)
            
         # transform response
         if status == 200:
-            return post_device_availability_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def create_websocket_token(self, url: str):  # noqa: E501
+    async def create_websocket_token(self, url: str) -> CreateWebsocketTokenResponse:  # noqa: E501
         """
         Create new websocket token for device
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(devices\/[^?]*?)(\/websocket)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/websocket'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="post")
            
         # transform response
         if status == 200:
-            return post_device_websocket_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def send_signaling_message(self, url: str, body: PostDeviceSignalingRequestBodyWrite, peerconnection_url: str):  # noqa: E501
+    async def send_signaling_message(self, url: str, body: SendSignalingMessageRequest, peerconnection_url: str) -> SendSignalingMessageResponse:  # noqa: E501
         """
         Send signaling message to device
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(devices\/[^?]*?)(\/signaling)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/signaling'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
 
-        # transform body
-        transformedBody = post_device_signaling_request_body_write_to_dict(body) if body else None
-
         # build query params
         query_params: Dict[str, Union[List[str], str]] = {}
         if peerconnection_url:
             if isinstance(peerconnection_url, list):
                 query_params['peerconnection_url'] = peerconnection_url
             else:
                 query_params['peerconnection_url'] = str(peerconnection_url)
+        
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody, params=query_params)
+        status, resp = await self._fetch(valid_url, method="post", body=body, params=query_params)
            
         # transform response
         if status == 200:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def list_peerconnections(self, url: str = "/peerconnections"):  # noqa: E501
+    async def list_peerconnections(self, url: str = "/peerconnections") -> ListPeerconnectionsResponse:  # noqa: E501
         """
         List Peer Connection
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(peerconnections)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/peerconnections'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_peerconnections_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def create_peerconnection(self, body: PostPeerconnectionsRequestBodyWrite, closedUrl: Optional[str] = None, statusChangedUrl: Optional[str] = None, url: str = "/peerconnections"):  # noqa: E501
+    async def create_peerconnection(self, body: CreatePeerconnectionRequest, url: str = "/peerconnections", closedUrl: Optional[str] = None, statusChangedUrl: Optional[str] = None) -> CreatePeerconnectionResponse:  # noqa: E501
         """
         Create a new Peer Connection
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(peerconnections)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/peerconnections'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
 
-        # transform body
-        transformedBody = post_peerconnections_request_body_write_to_dict(body) if body else None
-
         # build query params
         query_params: Dict[str, Union[List[str], str]] = {}
         if closedUrl:
             if isinstance(closedUrl, list):
                 query_params['closedUrl'] = closedUrl
             else:
                 query_params['closedUrl'] = str(closedUrl)
         if statusChangedUrl:
             if isinstance(statusChangedUrl, list):
                 query_params['statusChangedUrl'] = statusChangedUrl
             else:
                 query_params['statusChangedUrl'] = str(statusChangedUrl)
+        
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody, params=query_params)
+        status, resp = await self._fetch(valid_url, method="post", body=body, params=query_params)
            
         # transform response
         if status == 201:
-            return post_peerconnections_response_body201_read_from_dict(resp)
+            return resp
         if status == 202:
-            return post_peerconnections_response_body202_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def get_peerconnection(self, url: str):  # noqa: E501
+    async def get_peerconnection(self, url: str) -> GetPeerconnectionResponse:  # noqa: E501
         """
         View a peer connection
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(peerconnections\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_peerconnection_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def delete_peerconnection(self, url: str):  # noqa: E501
+    async def delete_peerconnection(self, url: str) -> DeletePeerconnectionResponse:  # noqa: E501
         """
         Delete a peer connection
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(peerconnections\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="delete")
            
         # transform response
         if status == 204:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def list_experiments(self, url: str = "/experiments"):  # noqa: E501
+    async def list_experiments(self, url: str = "/experiments") -> ListExperimentsResponse:  # noqa: E501
         """
         List experiments
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(experiments)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/experiments'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_experiments_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def create_experiment(self, body: PostExperimentsRequestBodyWrite, url: str = "/experiments"):  # noqa: E501
+    async def create_experiment(self, body: CreateExperimentRequest, url: str = "/experiments") -> CreateExperimentResponse:  # noqa: E501
         """
         Create a new experiment
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(experiments)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/experiments'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = post_experiments_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="post", body=body)
            
         # transform response
         if status == 201:
-            return post_experiments_response_body201_read_from_dict(resp)
+            return resp
         if status == 202:
-            return post_experiments_response_body202_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def get_experiment(self, url: str):  # noqa: E501
+    async def get_experiment(self, url: str) -> GetExperimentResponse:  # noqa: E501
         """
         View an experiment.
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(experiments\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_experiment_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def update_experiment(self, url: str, body: Optional[PatchExperimentRequestBodyWrite] = None, changedURL: Optional[str] = None):  # noqa: E501
+    async def update_experiment(self, url: str, body: Optional[UpdateExperimentRequest] = None, changedURL: Optional[str] = None) -> UpdateExperimentResponse:  # noqa: E501
         """
         Update an existing experiment.
         
         With this endpoint an experiment can be changed. The request body may be skipped if you just want to set a hook via the query string parameters.
         
         If a body is supplied you can choose to include any first level fields which will fully replace the field in the existing experiment.
         """  # noqa: E501
@@ -1244,228 +1243,209 @@
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(experiments\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
 
-        # transform body
-        transformedBody = patch_experiment_request_body_write_to_dict(body) if body else None
-
         # build query params
         query_params: Dict[str, Union[List[str], str]] = {}
         if changedURL:
             if isinstance(changedURL, list):
                 query_params['changedURL'] = changedURL
             else:
                 query_params['changedURL'] = str(changedURL)
+        
         # make http call
-        status, resp = await self._fetch(valid_url, method="patch", body=transformedBody, params=query_params)
+        status, resp = await self._fetch(valid_url, method="patch", body=body, params=query_params)
            
         # transform response
         if status == 200:
-            return patch_experiment_response_body200_read_from_dict(resp)
+            return resp
         if status == 202:
-            return patch_experiment_response_body202_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def delete_experiment(self, url: str):  # noqa: E501
+    async def delete_experiment(self, url: str) -> DeleteExperimentResponse:  # noqa: E501
         """
         Delete an experiment
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(experiments\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="delete")
            
         # transform response
         if status == 204:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def list_institutions(self, url: str = "/institutions"):  # noqa: E501
+    async def list_institutions(self, url: str = "/institutions") -> ListInstitutionsResponse:  # noqa: E501
         """
         List institutions
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(institutions)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/institutions'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_institutions_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def create_institution(self, body: PostInstitutionsRequestBodyWrite, url: str = "/institutions"):  # noqa: E501
+    async def create_institution(self, body: CreateInstitutionRequest, url: str = "/institutions") -> CreateInstitutionResponse:  # noqa: E501
         """
         Create a new institution
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(institutions)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/institutions'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = post_institutions_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="post", body=body)
            
         # transform response
         if status == 201:
-            return post_institutions_response_body201_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def get_institution(self, url: str):  # noqa: E501
+    async def get_institution(self, url: str) -> GetInstitutionResponse:  # noqa: E501
         """
         View an institution.
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(institutions\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_institution_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def update_institution(self, url: str, body: Optional[PatchInstitutionRequestBodyWrite] = None):  # noqa: E501
+    async def update_institution(self, url: str, body: Optional[UpdateInstitutionRequest] = None) -> UpdateInstitutionResponse:  # noqa: E501
         """
         Update an institution.
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(institutions\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = patch_institution_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="patch", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="patch", body=body)
            
         # transform response
         if status == 200:
-            return patch_institution_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def delete_institution(self, url: str):  # noqa: E501
+    async def delete_institution(self, url: str) -> DeleteInstitutionResponse:  # noqa: E501
         """
         Delete an institution
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(institutions\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="delete")
            
         # transform response
         if status == 204:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def list_updates(self, url: str = "/updates"):  # noqa: E501
+    async def list_updates(self, url: str = "/updates") -> ListUpdatesResponse:  # noqa: E501
         """
         Get update information for all devices
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(updates)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/updates'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="get")
            
         # transform response
         if status == 200:
-            return get_updates_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def create_update(self, body: PostUpdatesRequestBodyWrite, url: str = "/updates"):  # noqa: E501
+    async def create_update(self, body: CreateUpdateRequest, url: str = "/updates") -> CreateUpdateResponse:  # noqa: E501
         """
         Create new update information
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?()(updates)?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+'/updates'
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = post_updates_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="post", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="post", body=body)
            
         # transform response
         if status == 201:
-            return post_updates_response_body201_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def get_update(self, url: str, current_version: Optional[str] = None):  # noqa: E501
+    async def get_update(self, url: str, current_version: Optional[str] = None) -> GetUpdateResponse:  # noqa: E501
         """
         Get update for device
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
@@ -1479,65 +1459,61 @@
         # build query params
         query_params: Dict[str, Union[List[str], str]] = {}
         if current_version:
             if isinstance(current_version, list):
                 query_params['current_version'] = current_version
             else:
                 query_params['current_version'] = str(current_version)
+        
         # make http call
         status, resp = await self._fetch(valid_url, method="get", params=query_params)
            
         # transform response
         if status == 200:
-            return
+            return resp
         if status == 303:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def patch_update(self, url: str, body: PatchUpdateRequestBodyWrite):  # noqa: E501
+    async def patch_update(self, url: str, body: PatchUpdateRequest) -> PatchUpdateResponse:  # noqa: E501
         """
         Edit update information
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(updates\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
-        # transform body
-        transformedBody = patch_update_request_body_write_to_dict(body) if body else None
-
         # make http call
-        status, resp = await self._fetch(valid_url, method="patch", body=transformedBody)
+        status, resp = await self._fetch(valid_url, method="patch", body=body)
            
         # transform response
         if status == 200:
-            return patch_update_response_body200_read_from_dict(resp)
+            return resp
         raise Exception(f"Unexpected status code: {status}")
 
-    async def delete_update(self, url: str):  # noqa: E501
+    async def delete_update(self, url: str) -> DeleteUpdateResponse:  # noqa: E501
         """
         Delete update information
         """  # noqa: E501
         if not self.BASE_URL:
             raise Exception("No base url set")
 
         # match path to url schema
         m = re.search(r'^('+re.escape(self.BASE_URL)+r')?\/?(updates\/[^?]*?)()?$', url)
         if m is None:
             raise Exception("Invalid url")
         valid_url = '/'+m.group(2)+''
         if valid_url.startswith('//'):
             valid_url = valid_url[1:]
-
         # make http call
         status, resp = await self._fetch(valid_url, method="delete")
            
         # transform response
         if status == 204:
-            return
+            return resp
         raise Exception(f"Unexpected status code: {status}")
```

### Comparing `crosslab_api_client-0.2.1/tests/test_openapi.py` & `crosslab_api_client-0.2.2/tests/test_openapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import pytest
 from aioresponses import aioresponses
 import json
 import datetime
 
-from crosslab.api_client import APIClient
+from crosslab.api_client.client import APIClient
 from crosslab.api_client.schemas import *  # noqa: F403
 
 BASE_URL = 'https://api.example.com'
 
 
 def normalize_result(_dict):
     if isinstance(_dict, dict):
@@ -32,45 +32,46 @@
 
 @pytest.mark.asyncio
 async def test_login(aioresponses: aioresponses):
     url = r'/login'
     url_variant = r'login'
     full_url = BASE_URL+r'/login'
 
-    request_dict = json.loads(r'{"username":"aute in","password":"do in"}')
-    request = post_login_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"username":"aute in","password":"do in"}')
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_201_dict = json.loads(r'"voluptate Ut nulla aliquip"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.login(body=request, **parameters)
-            assert normalize_result(post_login_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'"voluptate Ut nulla aliquip"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.login(url=url, body=request, **parameters)
-            assert normalize_result(post_login_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'"voluptate Ut nulla aliquip"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.login(url=url_variant, body=request, **parameters)
-            assert normalize_result(post_login_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'"voluptate Ut nulla aliquip"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.login(url=full_url, body=request, **parameters)
-            assert normalize_result(post_login_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.login(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -86,14 +87,15 @@
                 resp = await client.login(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.login(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.login(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -109,14 +111,15 @@
                 resp = await client.login(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.login(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.login(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -132,14 +135,15 @@
                 resp = await client.login(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.login(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.login(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -155,14 +159,15 @@
                 resp = await client.login(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.login(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.login(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -186,18 +191,18 @@
 
 @pytest.mark.asyncio
 async def test_logout(aioresponses: aioresponses):
     url = r'/logout'
     url_variant = r'logout'
     full_url = BASE_URL+r'/logout'
 
-    request_dict = json.loads(r'{"token":"dolore"}')
-    request = post_logout_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"token":"dolore"}')
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=204)
         async with APIClient(BASE_URL) as client:
             resp = await client.logout(body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=204)
@@ -209,14 +214,15 @@
         async with APIClient(BASE_URL) as client:
             resp = await client.logout(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=204)
         async with APIClient(BASE_URL) as client:
             resp = await client.logout(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.logout(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -232,14 +238,15 @@
                 resp = await client.logout(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.logout(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.logout(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -255,14 +262,15 @@
                 resp = await client.logout(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.logout(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.logout(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -278,14 +286,15 @@
                 resp = await client.logout(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.logout(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.logout(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -301,14 +310,15 @@
                 resp = await client.logout(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.logout(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.logout(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -333,41 +343,43 @@
 @pytest.mark.asyncio
 async def test_create_device_authentication_token(aioresponses: aioresponses):
     url = r'/device_authentication_token'
     url_variant = r'device_authentication_token'
     full_url = BASE_URL+r'/device_authentication_token'
 
     parameter_list = [{"device_url": "test_string", }, ]
+
     for parameters in parameter_list:
         response_201_dict = json.loads(r'"consectetur in do nisi"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_device_authentication_token(**parameters)
-            assert normalize_result(post_device_authentication_token_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'"consectetur in do nisi"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_device_authentication_token(url=url, **parameters)
-            assert normalize_result(post_device_authentication_token_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'"consectetur in do nisi"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_device_authentication_token(url=url_variant, **parameters)
-            assert normalize_result(post_device_authentication_token_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'"consectetur in do nisi"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_device_authentication_token(url=full_url, **parameters)
-            assert normalize_result(post_device_authentication_token_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device_authentication_token(**parameters)
 
     for parameters in parameter_list:
@@ -383,14 +395,15 @@
                 resp = await client.create_device_authentication_token(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device_authentication_token(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device_authentication_token(**parameters)
 
     for parameters in parameter_list:
@@ -406,14 +419,15 @@
                 resp = await client.create_device_authentication_token(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device_authentication_token(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device_authentication_token(**parameters)
 
     for parameters in parameter_list:
@@ -429,14 +443,15 @@
                 resp = await client.create_device_authentication_token(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device_authentication_token(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device_authentication_token(**parameters)
 
     for parameters in parameter_list:
@@ -452,14 +467,15 @@
                 resp = await client.create_device_authentication_token(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device_authentication_token(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device_authentication_token(**parameters)
 
     for parameters in parameter_list:
@@ -484,41 +500,43 @@
 @pytest.mark.asyncio
 async def test_list_users(aioresponses: aioresponses):
     url = r'/users'
     url_variant = r'users'
     full_url = BASE_URL+r'/users'
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_users(**parameters)
-            assert normalize_result(get_users_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_users(url=url, **parameters)
-            assert normalize_result(get_users_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_users(url=url_variant, **parameters)
-            assert normalize_result(get_users_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_users(url=full_url, **parameters)
-            assert normalize_result(get_users_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_users(**parameters)
 
     for parameters in parameter_list:
@@ -534,14 +552,15 @@
                 resp = await client.list_users(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_users(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_users(**parameters)
 
     for parameters in parameter_list:
@@ -557,14 +576,15 @@
                 resp = await client.list_users(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_users(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_users(**parameters)
 
     for parameters in parameter_list:
@@ -580,14 +600,15 @@
                 resp = await client.list_users(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_users(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_users(**parameters)
 
     for parameters in parameter_list:
@@ -603,14 +624,15 @@
                 resp = await client.list_users(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_users(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_users(**parameters)
 
     for parameters in parameter_list:
@@ -634,45 +656,46 @@
 
 @pytest.mark.asyncio
 async def test_create_user(aioresponses: aioresponses):
     url = r'/users'
     url_variant = r'users'
     full_url = BASE_URL+r'/users'
 
-    request_dict = json.loads(r'{"username":"occaecat ex exercitation proident dolore","password":"laborum"}')
-    request = post_users_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"username":"occaecat ex exercitation proident dolore","password":"laborum"}')
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_user(body=request, **parameters)
-            assert normalize_result(post_users_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_user(url=url, body=request, **parameters)
-            assert normalize_result(post_users_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_user(url=url_variant, body=request, **parameters)
-            assert normalize_result(post_users_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_user(url=full_url, body=request, **parameters)
-            assert normalize_result(post_users_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_user(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -688,14 +711,15 @@
                 resp = await client.create_user(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_user(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_user(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -711,14 +735,15 @@
                 resp = await client.create_user(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_user(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_user(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -734,14 +759,15 @@
                 resp = await client.create_user(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_user(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_user(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -757,14 +783,15 @@
                 resp = await client.create_user(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_user(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_user(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -795,29 +822,29 @@
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_user(url=url, **parameters)
-            assert normalize_result(get_user_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_user(url=url_variant, **parameters)
-            assert normalize_result(get_user_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_user(url=full_url, **parameters)
-            assert normalize_result(get_user_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_user(url=url, **parameters)
 
@@ -908,39 +935,38 @@
 
 @pytest.mark.asyncio
 async def test_update_user(aioresponses: aioresponses):
     url = r'/users/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'users/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/users/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
-    request_dict = json.loads(r'{"username":"tempor","password":"ad"}')
-    request = patch_user_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"username":"tempor","password":"ad"}')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_user(url=url, body=request, **parameters)
-            assert normalize_result(patch_user_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_user(url=url_variant, body=request, **parameters)
-            assert normalize_result(patch_user_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_user(url=full_url, body=request, **parameters)
-            assert normalize_result(patch_user_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_user(url=url, body=request, **parameters)
 
@@ -1152,29 +1178,29 @@
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_roles_of_user(url=url, **parameters)
-            assert normalize_result(get_user_roles_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_roles_of_user(url=url_variant, **parameters)
-            assert normalize_result(get_user_roles_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_roles_of_user(url=full_url, **parameters)
-            assert normalize_result(get_user_roles_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_roles_of_user(url=url, **parameters)
 
@@ -1265,16 +1291,15 @@
 
 @pytest.mark.asyncio
 async def test_add_roles_to_user(aioresponses: aioresponses):
     url = r'/users/c799cc2e-cdc5-4143-973a-6f56a5afa82c/roles'
     url_variant = r'users/c799cc2e-cdc5-4143-973a-6f56a5afa82c/roles'
     full_url = BASE_URL+r'/users/c799cc2e-cdc5-4143-973a-6f56a5afa82c/roles'
 
-    request_dict = json.loads(r'["enim","consequat aute Ut sit anim"]')
-    request = post_user_roles_request_body_write_from_dict(request_dict)
+    request = json.loads(r'["enim","consequat aute Ut sit anim"]')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=204)
         async with APIClient(BASE_URL) as client:
             resp = await client.add_roles_to_user(url=url, body=request, **parameters)
@@ -1382,16 +1407,15 @@
 
 @pytest.mark.asyncio
 async def test_remove_roles_from_user(aioresponses: aioresponses):
     url = r'/users/c799cc2e-cdc5-4143-973a-6f56a5afa82c/roles'
     url_variant = r'users/c799cc2e-cdc5-4143-973a-6f56a5afa82c/roles'
     full_url = BASE_URL+r'/users/c799cc2e-cdc5-4143-973a-6f56a5afa82c/roles'
 
-    request_dict = json.loads(r'["enim","consequat aute Ut sit anim"]')
-    request = delete_user_roles_request_body_write_from_dict(request_dict)
+    request = json.loads(r'["enim","consequat aute Ut sit anim"]')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         aioresponses.delete(re.compile(re.escape(full_url)+r'(\?.*)?'), status=204)
         async with APIClient(BASE_URL) as client:
             resp = await client.remove_roles_from_user(url=url, body=request, **parameters)
@@ -1500,41 +1524,43 @@
 @pytest.mark.asyncio
 async def test_list_roles(aioresponses: aioresponses):
     url = r'/roles'
     url_variant = r'roles'
     full_url = BASE_URL+r'/roles'
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_roles(**parameters)
-            assert normalize_result(get_roles_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_roles(url=url, **parameters)
-            assert normalize_result(get_roles_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_roles(url=url_variant, **parameters)
-            assert normalize_result(get_roles_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"id":"nisi nostrud nulla sit","url":"https://aeUhNJdx.hxjnM137Xzngz--,VAiwP","name":"ipsum ullamco in","scopes":["Ut Duis","non consequat labore dolor Duis","anim elit sed nisi","Ut sunt exercitation non"]},{"name":"mollit qui enim ad Ut","id":"in ut eiusmod"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_roles(url=full_url, **parameters)
-            assert normalize_result(get_roles_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_roles(**parameters)
 
     for parameters in parameter_list:
@@ -1550,14 +1576,15 @@
                 resp = await client.list_roles(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_roles(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_roles(**parameters)
 
     for parameters in parameter_list:
@@ -1573,14 +1600,15 @@
                 resp = await client.list_roles(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_roles(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_roles(**parameters)
 
     for parameters in parameter_list:
@@ -1596,14 +1624,15 @@
                 resp = await client.list_roles(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_roles(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_roles(**parameters)
 
     for parameters in parameter_list:
@@ -1619,14 +1648,15 @@
                 resp = await client.list_roles(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_roles(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_roles(**parameters)
 
     for parameters in parameter_list:
@@ -1650,45 +1680,46 @@
 
 @pytest.mark.asyncio
 async def test_create_role(aioresponses: aioresponses):
     url = r'/roles'
     url_variant = r'roles'
     full_url = BASE_URL+r'/roles'
 
-    request_dict = json.loads(r'{"name":"nulla nisi","scopes":["in amet et in","cupidatat","adipisicing ad","dolore aliqua in","Ut esse ad"]}')
-    request = post_roles_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"name":"nulla nisi","scopes":["in amet et in","cupidatat","adipisicing ad","dolore aliqua in","Ut esse ad"]}')
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_role(body=request, **parameters)
-            assert normalize_result(post_roles_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_role(url=url, body=request, **parameters)
-            assert normalize_result(post_roles_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_role(url=url_variant, body=request, **parameters)
-            assert normalize_result(post_roles_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_role(url=full_url, body=request, **parameters)
-            assert normalize_result(post_roles_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_role(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -1704,14 +1735,15 @@
                 resp = await client.create_role(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_role(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_role(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -1727,14 +1759,15 @@
                 resp = await client.create_role(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_role(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_role(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -1750,14 +1783,15 @@
                 resp = await client.create_role(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_role(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_role(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -1773,14 +1807,15 @@
                 resp = await client.create_role(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_role(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_role(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -1811,29 +1846,29 @@
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_role(url=url, **parameters)
-            assert normalize_result(get_role_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_role(url=url_variant, **parameters)
-            assert normalize_result(get_role_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_role(url=full_url, **parameters)
-            assert normalize_result(get_role_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_role(url=url, **parameters)
 
@@ -1924,39 +1959,38 @@
 
 @pytest.mark.asyncio
 async def test_update_role(aioresponses: aioresponses):
     url = r'/roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
-    request_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
-    request = patch_role_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_role(url=url, body=request, **parameters)
-            assert normalize_result(patch_role_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_role(url=url_variant, body=request, **parameters)
-            assert normalize_result(patch_role_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"scopes":["dolor commodo id in","ut"],"name":"commodo ad nulla nisi et"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_role(url=full_url, body=request, **parameters)
-            assert normalize_result(patch_role_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_role(url=url, body=request, **parameters)
 
@@ -2168,29 +2202,29 @@
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_users_with_role(url=url, **parameters)
-            assert normalize_result(get_role_users_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_users_with_role(url=url_variant, **parameters)
-            assert normalize_result(get_role_users_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"roles":[{"url":"https://DeURFWCx.onpu.Mw7RTfb2f0l1WRLzoCO5oU","id":"enim anim","name":"non incididunt Duis pariatur minim","scopes":["anim voluptate aute Duis"]}],"url":"https://dhvskgVWHiqwVntPoDQGF.ovePGeHEMw62XGwjeRU8wlzpIq5MThVrmqRhgckA-PLHLyY,zw+oQY"},{"roles":[{"url":"http://guBFBXETlaqfTdLLERbYNLLxZfDPO.cpikrn3,,iXCReR4ttNoe-tMnW,hKH1KPFSPED.4dVYJyHO3rzehHFgRkEY5teKM06BwHocOzVHwyg,"}],"password":"elit esse aute","username":"culpa","url":"http://ulxpvZToDIljIFfbjoFuAGBWNAOtS.fqegaiBJIsMZvyhownQK8JUbyjybkXJh,jzugkWn1ynn,-Ns3FAcYzdlQsMoygSVAjcS"},{"username":"proident Ut ad reprehenderit","roles":[{"url":"http://YfHcCjfNllGG.jvkhcj3bIX7FusXR++ln7ptUnTRvS9tw"},{"name":"aliquip ullamco culpa consequat","id":"in adipisicing","url":"https://PSkjL.rbUkxB9XvO+SAZ-s5iURdPqEn88GdVFYDNTUhtH8XsdZNZFuVC"},{"url":"http://vPvLleEDIbPSRvhKNMrErekJWIK.eibvkaeIbOawfCEA4OcE8mDAn8qofAP0Vr3cpaxvhabQWVecNZOqDCz5oJ3","scopes":["veniam non ut","exercitation commodo elit","adipisicing tempor","cupidatat Ut dolor reprehenderit","reprehenderit ut ipsum et cupidatat"],"id":"velit Excepteur occaecat"}],"url":"https://GXYKIhsWipBeJUIcBNukIdJE.hvVmOk85dI5oEflv,EDD+0-eJOa2qdHKltLPwsg9GJbzaQtJhzdVuNw3KucXXHSJzZckeMPFcGv"},{"roles":[{"url":"https://zjihqqLRdlnACjMmxxukpKeC.dovQ0iw-ZmN6q8sTZyw6F0FTZSbziJGvEeIVH1GN0ttobx0vNnfyrpwTmV5TmlGc2KNvdrmx","id":"elit sint non consectetur do","name":"laborum incididunt exercitation","scopes":["fugiat aute eiusmod aliquip","in eu Lorem","voluptate incididunt dolore dolore"]},{"url":"http://fcJDGAMVZZteWEL.lrZBLoqWr,-OhEIp52w5ni6b1KGQTs.B","scopes":["id labore ut voluptate","ex magna deserunt culpa Ut","aliquip","eu adipisicing dolore aliqua reprehenderit","elit enim commodo"]}],"password":"dolore in","id":"Excepteur dolor consectetur cupidatat","url":"https://LsSgDHAqAGEtaRzEMBLYlkq.keaOZMqdQo6mUVs3RF6NaIKRDy45Edaa6bLzykKVsfHjYxnH+qEgP5HsYmgYrYeX4","username":"cupidatat nostrud esse dolore nulla"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_users_with_role(url=full_url, **parameters)
-            assert normalize_result(get_role_users_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_users_with_role(url=url, **parameters)
 
@@ -2281,16 +2315,15 @@
 
 @pytest.mark.asyncio
 async def test_add_users_to_role(aioresponses: aioresponses):
     url = r'/roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c/users'
     url_variant = r'roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c/users'
     full_url = BASE_URL+r'/roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c/users'
 
-    request_dict = json.loads(r'["enim","consequat aute Ut sit anim"]')
-    request = post_role_users_request_body_write_from_dict(request_dict)
+    request = json.loads(r'["enim","consequat aute Ut sit anim"]')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=204)
         async with APIClient(BASE_URL) as client:
             resp = await client.add_users_to_role(url=url, body=request, **parameters)
@@ -2398,16 +2431,15 @@
 
 @pytest.mark.asyncio
 async def test_remove_users_from_role(aioresponses: aioresponses):
     url = r'/roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c/users'
     url_variant = r'roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c/users'
     full_url = BASE_URL+r'/roles/c799cc2e-cdc5-4143-973a-6f56a5afa82c/users'
 
-    request_dict = json.loads(r'["enim","consequat aute Ut sit anim"]')
-    request = delete_role_users_request_body_write_from_dict(request_dict)
+    request = json.loads(r'["enim","consequat aute Ut sit anim"]')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         aioresponses.delete(re.compile(re.escape(full_url)+r'(\?.*)?'), status=204)
         async with APIClient(BASE_URL) as client:
             resp = await client.remove_users_from_role(url=url, body=request, **parameters)
@@ -2516,41 +2548,43 @@
 @pytest.mark.asyncio
 async def test_get_identity(aioresponses: aioresponses):
     url = r'/identity'
     url_variant = r'identity'
     full_url = BASE_URL+r'/identity'
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_identity(**parameters)
-            assert normalize_result(get_identity_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_identity(url=url, **parameters)
-            assert normalize_result(get_identity_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_identity(url=url_variant, **parameters)
-            assert normalize_result(get_identity_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_identity(url=full_url, **parameters)
-            assert normalize_result(get_identity_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_identity(**parameters)
 
     for parameters in parameter_list:
@@ -2566,14 +2600,15 @@
                 resp = await client.get_identity(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_identity(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_identity(**parameters)
 
     for parameters in parameter_list:
@@ -2589,14 +2624,15 @@
                 resp = await client.get_identity(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_identity(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_identity(**parameters)
 
     for parameters in parameter_list:
@@ -2612,14 +2648,15 @@
                 resp = await client.get_identity(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_identity(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_identity(**parameters)
 
     for parameters in parameter_list:
@@ -2635,14 +2672,15 @@
                 resp = await client.get_identity(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_identity(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_identity(**parameters)
 
     for parameters in parameter_list:
@@ -2666,45 +2704,46 @@
 
 @pytest.mark.asyncio
 async def test_update_identity(aioresponses: aioresponses):
     url = r'/identity'
     url_variant = r'identity'
     full_url = BASE_URL+r'/identity'
 
-    request_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
-    request = patch_identity_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_identity(body=request, **parameters)
-            assert normalize_result(patch_identity_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_identity(url=url, body=request, **parameters)
-            assert normalize_result(patch_identity_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_identity(url=url_variant, body=request, **parameters)
-            assert normalize_result(patch_identity_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"url":"https://wjhCRJVAMrw.qsvc6FSHdo,VugWBeX,e5eUtd-dX6uBD2M7ZYriEcfD+","id":"Lorem","username":"enim magna eu","password":"ut elit quis anim","roles":[{"scopes":["magna culpa dolore","ad laboris amet","laboris","deserunt ullamco eiusmod voluptate","Excepteur ipsum consequat nisi exercitation"],"url":"http://hHdqGncjesLInHvCUzWEKnM.adcCMugPEJR,2x+RQlqh,QgDtridgq","name":"irure magna sed et","id":"ipsum"},{"url":"http://DszIzhdPiXvExSMPFsYnovghHvYrW.joDZz,Yq-izLjyXwqxBdI16MCIOUT31qScyrQBgqbR","id":"deserunt est aliqua","name":"dolore consectetur commodo"}]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_identity(url=full_url, body=request, **parameters)
-            assert normalize_result(patch_identity_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
+
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_identity(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -2720,14 +2759,15 @@
                 resp = await client.update_identity(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_identity(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_identity(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -2743,14 +2783,15 @@
                 resp = await client.update_identity(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_identity(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_identity(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -2766,14 +2807,15 @@
                 resp = await client.update_identity(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_identity(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_identity(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -2789,14 +2831,15 @@
                 resp = await client.update_identity(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_identity(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_identity(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -2820,45 +2863,46 @@
 
 @pytest.mark.asyncio
 async def test_get_schedule(aioresponses: aioresponses):
     url = r'/schedule'
     url_variant = r'schedule'
     full_url = BASE_URL+r'/schedule'
 
-    request_dict = json.loads(r'{"Experiment":{"Devices":[{"ID":"https://cHaylvBKdWJSNBxjFMsRIFtEoQDGDi.kucakbCJEWoYBT7b+w9mFqQ"}],"Description":"veniam dolore elit incididunt aliquip"},"Time":{"Start":"2013-01-14T23:45:15.0Z","End":"2009-06-17T21:25:10.0Z"},"Combined":true,"onlyOwn":true}')
-    request = post_schedule_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"Experiment":{"Devices":[{"ID":"https://cHaylvBKdWJSNBxjFMsRIFtEoQDGDi.kucakbCJEWoYBT7b+w9mFqQ"}],"Description":"veniam dolore elit incididunt aliquip"},"Time":{"Start":"2013-01-14T23:45:15.0Z","End":"2009-06-17T21:25:10.0Z"},"Combined":true,"onlyOwn":true}')
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"Device":"deserunt","Booked":[{"Start":"1948-05-28T02:28:12.0Z","End":"2011-12-30T01:38:02.0Z"},{"Start":"1985-12-18T10:09:01.0Z","End":"1978-01-18T18:32:01.0Z"}],"Free":[{"Start":"1961-12-22T19:04:41.0Z","End":"2001-11-27T06:05:08.0Z"},{"Start":"2012-02-02T16:18:57.0Z","End":"1966-03-15T22:35:31.0Z"},{"Start":"1982-08-02T04:58:59.0Z","End":"1994-05-06T05:04:50.0Z"},{"Start":"2008-12-26T17:21:24.0Z","End":"1983-12-05T17:38:55.0Z"}]},{"Device":"voluptate sed","Booked":[{"Start":"2013-11-17T05:48:45.0Z","End":"1998-12-07T01:30:34.0Z"},{"Start":"1984-09-11T04:11:16.0Z","End":"1970-10-28T01:19:38.0Z"},{"Start":"1958-04-10T07:56:51.0Z","End":"1960-07-18T04:47:46.0Z"}],"Free":[{"Start":"1982-08-29T04:12:21.0Z","End":"1968-11-30T13:07:01.0Z"}]},{"Device":"irure laboris consequat minim","Booked":[{"Start":"2010-02-25T04:35:02.0Z","End":"1959-09-10T01:34:53.0Z"}],"Free":[{"Start":"2001-04-09T22:29:19.0Z","End":"2005-06-04T08:28:39.0Z"},{"Start":"1979-01-07T05:35:26.0Z","End":"2019-06-10T21:57:56.0Z"},{"Start":"1971-01-18T04:03:03.0Z","End":"1960-05-19T05:07:48.0Z"}]},{"Device":"est et","Booked":[{"Start":"1969-01-26T21:55:52.0Z","End":"2014-09-15T10:37:51.0Z"},{"Start":"1976-11-11T14:44:42.0Z","End":"2013-12-15T19:03:32.0Z"}],"Free":[{"Start":"1963-05-16T13:25:55.0Z","End":"2011-06-21T19:03:17.0Z"},{"Start":"1944-05-29T20:44:47.0Z","End":"1962-03-04T14:52:27.0Z"},{"Start":"1977-04-02T14:22:19.0Z","End":"2011-07-11T16:07:14.0Z"}]}]')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_schedule(body=request, **parameters)
-            assert normalize_result(post_schedule_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"Device":"deserunt","Booked":[{"Start":"1948-05-28T02:28:12.0Z","End":"2011-12-30T01:38:02.0Z"},{"Start":"1985-12-18T10:09:01.0Z","End":"1978-01-18T18:32:01.0Z"}],"Free":[{"Start":"1961-12-22T19:04:41.0Z","End":"2001-11-27T06:05:08.0Z"},{"Start":"2012-02-02T16:18:57.0Z","End":"1966-03-15T22:35:31.0Z"},{"Start":"1982-08-02T04:58:59.0Z","End":"1994-05-06T05:04:50.0Z"},{"Start":"2008-12-26T17:21:24.0Z","End":"1983-12-05T17:38:55.0Z"}]},{"Device":"voluptate sed","Booked":[{"Start":"2013-11-17T05:48:45.0Z","End":"1998-12-07T01:30:34.0Z"},{"Start":"1984-09-11T04:11:16.0Z","End":"1970-10-28T01:19:38.0Z"},{"Start":"1958-04-10T07:56:51.0Z","End":"1960-07-18T04:47:46.0Z"}],"Free":[{"Start":"1982-08-29T04:12:21.0Z","End":"1968-11-30T13:07:01.0Z"}]},{"Device":"irure laboris consequat minim","Booked":[{"Start":"2010-02-25T04:35:02.0Z","End":"1959-09-10T01:34:53.0Z"}],"Free":[{"Start":"2001-04-09T22:29:19.0Z","End":"2005-06-04T08:28:39.0Z"},{"Start":"1979-01-07T05:35:26.0Z","End":"2019-06-10T21:57:56.0Z"},{"Start":"1971-01-18T04:03:03.0Z","End":"1960-05-19T05:07:48.0Z"}]},{"Device":"est et","Booked":[{"Start":"1969-01-26T21:55:52.0Z","End":"2014-09-15T10:37:51.0Z"},{"Start":"1976-11-11T14:44:42.0Z","End":"2013-12-15T19:03:32.0Z"}],"Free":[{"Start":"1963-05-16T13:25:55.0Z","End":"2011-06-21T19:03:17.0Z"},{"Start":"1944-05-29T20:44:47.0Z","End":"1962-03-04T14:52:27.0Z"},{"Start":"1977-04-02T14:22:19.0Z","End":"2011-07-11T16:07:14.0Z"}]}]')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_schedule(url=url, body=request, **parameters)
-            assert normalize_result(post_schedule_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"Device":"deserunt","Booked":[{"Start":"1948-05-28T02:28:12.0Z","End":"2011-12-30T01:38:02.0Z"},{"Start":"1985-12-18T10:09:01.0Z","End":"1978-01-18T18:32:01.0Z"}],"Free":[{"Start":"1961-12-22T19:04:41.0Z","End":"2001-11-27T06:05:08.0Z"},{"Start":"2012-02-02T16:18:57.0Z","End":"1966-03-15T22:35:31.0Z"},{"Start":"1982-08-02T04:58:59.0Z","End":"1994-05-06T05:04:50.0Z"},{"Start":"2008-12-26T17:21:24.0Z","End":"1983-12-05T17:38:55.0Z"}]},{"Device":"voluptate sed","Booked":[{"Start":"2013-11-17T05:48:45.0Z","End":"1998-12-07T01:30:34.0Z"},{"Start":"1984-09-11T04:11:16.0Z","End":"1970-10-28T01:19:38.0Z"},{"Start":"1958-04-10T07:56:51.0Z","End":"1960-07-18T04:47:46.0Z"}],"Free":[{"Start":"1982-08-29T04:12:21.0Z","End":"1968-11-30T13:07:01.0Z"}]},{"Device":"irure laboris consequat minim","Booked":[{"Start":"2010-02-25T04:35:02.0Z","End":"1959-09-10T01:34:53.0Z"}],"Free":[{"Start":"2001-04-09T22:29:19.0Z","End":"2005-06-04T08:28:39.0Z"},{"Start":"1979-01-07T05:35:26.0Z","End":"2019-06-10T21:57:56.0Z"},{"Start":"1971-01-18T04:03:03.0Z","End":"1960-05-19T05:07:48.0Z"}]},{"Device":"est et","Booked":[{"Start":"1969-01-26T21:55:52.0Z","End":"2014-09-15T10:37:51.0Z"},{"Start":"1976-11-11T14:44:42.0Z","End":"2013-12-15T19:03:32.0Z"}],"Free":[{"Start":"1963-05-16T13:25:55.0Z","End":"2011-06-21T19:03:17.0Z"},{"Start":"1944-05-29T20:44:47.0Z","End":"1962-03-04T14:52:27.0Z"},{"Start":"1977-04-02T14:22:19.0Z","End":"2011-07-11T16:07:14.0Z"}]}]')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_schedule(url=url_variant, body=request, **parameters)
-            assert normalize_result(post_schedule_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"Device":"deserunt","Booked":[{"Start":"1948-05-28T02:28:12.0Z","End":"2011-12-30T01:38:02.0Z"},{"Start":"1985-12-18T10:09:01.0Z","End":"1978-01-18T18:32:01.0Z"}],"Free":[{"Start":"1961-12-22T19:04:41.0Z","End":"2001-11-27T06:05:08.0Z"},{"Start":"2012-02-02T16:18:57.0Z","End":"1966-03-15T22:35:31.0Z"},{"Start":"1982-08-02T04:58:59.0Z","End":"1994-05-06T05:04:50.0Z"},{"Start":"2008-12-26T17:21:24.0Z","End":"1983-12-05T17:38:55.0Z"}]},{"Device":"voluptate sed","Booked":[{"Start":"2013-11-17T05:48:45.0Z","End":"1998-12-07T01:30:34.0Z"},{"Start":"1984-09-11T04:11:16.0Z","End":"1970-10-28T01:19:38.0Z"},{"Start":"1958-04-10T07:56:51.0Z","End":"1960-07-18T04:47:46.0Z"}],"Free":[{"Start":"1982-08-29T04:12:21.0Z","End":"1968-11-30T13:07:01.0Z"}]},{"Device":"irure laboris consequat minim","Booked":[{"Start":"2010-02-25T04:35:02.0Z","End":"1959-09-10T01:34:53.0Z"}],"Free":[{"Start":"2001-04-09T22:29:19.0Z","End":"2005-06-04T08:28:39.0Z"},{"Start":"1979-01-07T05:35:26.0Z","End":"2019-06-10T21:57:56.0Z"},{"Start":"1971-01-18T04:03:03.0Z","End":"1960-05-19T05:07:48.0Z"}]},{"Device":"est et","Booked":[{"Start":"1969-01-26T21:55:52.0Z","End":"2014-09-15T10:37:51.0Z"},{"Start":"1976-11-11T14:44:42.0Z","End":"2013-12-15T19:03:32.0Z"}],"Free":[{"Start":"1963-05-16T13:25:55.0Z","End":"2011-06-21T19:03:17.0Z"},{"Start":"1944-05-29T20:44:47.0Z","End":"1962-03-04T14:52:27.0Z"},{"Start":"1977-04-02T14:22:19.0Z","End":"2011-07-11T16:07:14.0Z"}]}]')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_schedule(url=full_url, body=request, **parameters)
-            assert normalize_result(post_schedule_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_schedule(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -2874,14 +2918,15 @@
                 resp = await client.get_schedule(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_schedule(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_schedule(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -2897,14 +2942,15 @@
                 resp = await client.get_schedule(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_schedule(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         response_404_dict = json.loads(r'"commodo in"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404, payload=response_404_dict)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_schedule(body=request, **parameters)
 
@@ -2924,14 +2970,15 @@
 
     for parameters in parameter_list:
         response_404_dict = json.loads(r'"commodo in"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404, payload=response_404_dict)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_schedule(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         response_422_dict = json.loads(r'"mollit"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=422, payload=response_422_dict)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_schedule(body=request, **parameters)
 
@@ -2951,14 +2998,15 @@
 
     for parameters in parameter_list:
         response_422_dict = json.loads(r'"mollit"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=422, payload=response_422_dict)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_schedule(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         response_500_dict = json.loads(r'"veniam ex eu"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500, payload=response_500_dict)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_schedule(body=request, **parameters)
 
@@ -2978,14 +3026,15 @@
 
     for parameters in parameter_list:
         response_500_dict = json.loads(r'"veniam ex eu"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500, payload=response_500_dict)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_schedule(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=503)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_schedule(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -3009,45 +3058,46 @@
 
 @pytest.mark.asyncio
 async def test_book_experiment(aioresponses: aioresponses):
     url = r'/booking'
     url_variant = r'booking'
     full_url = BASE_URL+r'/booking'
 
-    request_dict = json.loads(r'{"Experiment":{"Devices":[{"ID":"https://egpZNfFBa.tvnlNGgk0v"},{"ID":"https://buBjeTLpmnTgKUztkGK.pqvsEwkiZmyNgeSImHsnvoQUf.3KIvtTb"}]},"Time":{"Start":"1947-01-15T03:43:26.0Z","End":"1952-10-14T16:17:07.0Z"},"Type":"normal"}')
-    request = post_booking_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"Experiment":{"Devices":[{"ID":"https://egpZNfFBa.tvnlNGgk0v"},{"ID":"https://buBjeTLpmnTgKUztkGK.pqvsEwkiZmyNgeSImHsnvoQUf.3KIvtTb"}]},"Time":{"Start":"1947-01-15T03:43:26.0Z","End":"1952-10-14T16:17:07.0Z"},"Type":"normal"}')
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"BookingID":"https://zurWHxnuNekdQetiawWc.uncovYoMyvENFntDMplEsNtcFgBUP17FfZ2Wkcx1SeQnu+iggAOfJGk"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.book_experiment(body=request, **parameters)
-            assert normalize_result(post_booking_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"BookingID":"https://zurWHxnuNekdQetiawWc.uncovYoMyvENFntDMplEsNtcFgBUP17FfZ2Wkcx1SeQnu+iggAOfJGk"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.book_experiment(url=url, body=request, **parameters)
-            assert normalize_result(post_booking_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"BookingID":"https://zurWHxnuNekdQetiawWc.uncovYoMyvENFntDMplEsNtcFgBUP17FfZ2Wkcx1SeQnu+iggAOfJGk"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.book_experiment(url=url_variant, body=request, **parameters)
-            assert normalize_result(post_booking_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"BookingID":"https://zurWHxnuNekdQetiawWc.uncovYoMyvENFntDMplEsNtcFgBUP17FfZ2Wkcx1SeQnu+iggAOfJGk"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.book_experiment(url=full_url, body=request, **parameters)
-            assert normalize_result(post_booking_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.book_experiment(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -3063,14 +3113,15 @@
                 resp = await client.book_experiment(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.book_experiment(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         response_500_dict = json.loads(r'"ea mollit"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500, payload=response_500_dict)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.book_experiment(body=request, **parameters)
 
@@ -3090,14 +3141,15 @@
 
     for parameters in parameter_list:
         response_500_dict = json.loads(r'"ea mollit"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500, payload=response_500_dict)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.book_experiment(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=503)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.book_experiment(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -3121,39 +3173,38 @@
 
 @pytest.mark.asyncio
 async def test_update_booking(aioresponses: aioresponses):
     url = r'/booking/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'booking/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/booking/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
-    request_dict = json.loads(r'{}')
-    request = patch_booking_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{}')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"BookingID":"http://akJjTPgNsQCcPFMaZe.zlmvloXia0bqBjdT1Rfy3PSFGpCVkgqoAa9GgiZHg4r"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_booking(url=url, body=request, **parameters)
-            assert normalize_result(patch_booking_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"BookingID":"http://akJjTPgNsQCcPFMaZe.zlmvloXia0bqBjdT1Rfy3PSFGpCVkgqoAa9GgiZHg4r"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_booking(url=url_variant, body=request, **parameters)
-            assert normalize_result(patch_booking_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"BookingID":"http://akJjTPgNsQCcPFMaZe.zlmvloXia0bqBjdT1Rfy3PSFGpCVkgqoAa9GgiZHg4r"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_booking(url=full_url, body=request, **parameters)
-            assert normalize_result(patch_booking_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_booking(url=url, body=request, **parameters)
 
@@ -3353,29 +3404,29 @@
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"Booking":{"ID":"http://meMsm.xdigcAH1DeqS7KYg00WMVFvdHFi9jENfN","Time":{"Start":"2003-12-05T17:28:14.0Z","End":"1989-09-22T05:58:40.0Z"},"Devices":["https://AYKQXTFTAgMPOcXJuFVwxQmupPoOCjX.hkkyfuLSxo4lm2Iwil1QaifOIqKj2zjsJq9oZuORAi","http://enbJtSBUvWZK.dydyTKbknuYuIPvFzBhOYI82qnBEvaAxDzF,v-ZNsdk1rfaRChhXMqKKQXaKob"],"Status":"pending","You":true,"External":true,"Message":"sed sunt non enim occaecat"},"Locked":false}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_booking(url=url, **parameters)
-            assert normalize_result(get_booking_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"Booking":{"ID":"http://meMsm.xdigcAH1DeqS7KYg00WMVFvdHFi9jENfN","Time":{"Start":"2003-12-05T17:28:14.0Z","End":"1989-09-22T05:58:40.0Z"},"Devices":["https://AYKQXTFTAgMPOcXJuFVwxQmupPoOCjX.hkkyfuLSxo4lm2Iwil1QaifOIqKj2zjsJq9oZuORAi","http://enbJtSBUvWZK.dydyTKbknuYuIPvFzBhOYI82qnBEvaAxDzF,v-ZNsdk1rfaRChhXMqKKQXaKob"],"Status":"pending","You":true,"External":true,"Message":"sed sunt non enim occaecat"},"Locked":false}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_booking(url=url_variant, **parameters)
-            assert normalize_result(get_booking_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"Booking":{"ID":"http://meMsm.xdigcAH1DeqS7KYg00WMVFvdHFi9jENfN","Time":{"Start":"2003-12-05T17:28:14.0Z","End":"1989-09-22T05:58:40.0Z"},"Devices":["https://AYKQXTFTAgMPOcXJuFVwxQmupPoOCjX.hkkyfuLSxo4lm2Iwil1QaifOIqKj2zjsJq9oZuORAi","http://enbJtSBUvWZK.dydyTKbknuYuIPvFzBhOYI82qnBEvaAxDzF,v-ZNsdk1rfaRChhXMqKKQXaKob"],"Status":"pending","You":true,"External":true,"Message":"sed sunt non enim occaecat"},"Locked":false}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_booking(url=full_url, **parameters)
-            assert normalize_result(get_booking_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_booking(url=url, **parameters)
 
@@ -3575,29 +3626,29 @@
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"Booking":{"ID":"http://yoMAnxJpiGEEkJWmzKnSqBtqhCnvIdMSr.cbrqcVvPcrHoB7.QLta4DcDk.jczRQZu-TfKCushfW+nJ6G0o2G1leLXCDu3a42jPisVbqbz","Time":{"Start":"1991-10-08T01:22:07.0Z","End":"2022-11-10T18:20:43.0Z"},"Devices":["https://xqNbClEPdpHKig.dhiiSiYrU3DYITw6tF1lmUdif8O07Y.LfqivCk3JNt7iUd9J,N4eDsNZfLZ70M","https://yTxELhUrJEDpBapgc.ttgsbLDKBsuj096crVKGCv,kj,hrV-RVDFyUhRLpwvGOaInHu1ZSt1drc5","http://urgvYKPgJ.wss5xn,ZSCgIP5RqnKMw5sFSj27mwK6wfLkBSkbnpwsw2hYZFqmdh+80zT-NM"],"Status":"active","You":false,"External":true,"Message":"Lorem ipsum incididunt","Type":"normal"},"Time":{"Start":"1983-04-17T07:30:29.0Z","End":"2022-12-07T12:03:19.0Z"},"Tokens":[{"Token":"ea Duis anim"},{"Device":"https://lujjGqZNTwEvcLV.nyfEzuMfcb,byZ1.XCuvg+T","Token":"consectetur aute nisi"},{"Device":"https://kFwUbbqqJHNFECezWeTvNmjTlr.ymDXzxt7.mNmOJ7P,4rOs","Token":"cillum sunt qui Lorem dolor"}]}')
         aioresponses.put(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.lock_booking(url=url, **parameters)
-            assert normalize_result(put_booking_lock_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"Booking":{"ID":"http://yoMAnxJpiGEEkJWmzKnSqBtqhCnvIdMSr.cbrqcVvPcrHoB7.QLta4DcDk.jczRQZu-TfKCushfW+nJ6G0o2G1leLXCDu3a42jPisVbqbz","Time":{"Start":"1991-10-08T01:22:07.0Z","End":"2022-11-10T18:20:43.0Z"},"Devices":["https://xqNbClEPdpHKig.dhiiSiYrU3DYITw6tF1lmUdif8O07Y.LfqivCk3JNt7iUd9J,N4eDsNZfLZ70M","https://yTxELhUrJEDpBapgc.ttgsbLDKBsuj096crVKGCv,kj,hrV-RVDFyUhRLpwvGOaInHu1ZSt1drc5","http://urgvYKPgJ.wss5xn,ZSCgIP5RqnKMw5sFSj27mwK6wfLkBSkbnpwsw2hYZFqmdh+80zT-NM"],"Status":"active","You":false,"External":true,"Message":"Lorem ipsum incididunt","Type":"normal"},"Time":{"Start":"1983-04-17T07:30:29.0Z","End":"2022-12-07T12:03:19.0Z"},"Tokens":[{"Token":"ea Duis anim"},{"Device":"https://lujjGqZNTwEvcLV.nyfEzuMfcb,byZ1.XCuvg+T","Token":"consectetur aute nisi"},{"Device":"https://kFwUbbqqJHNFECezWeTvNmjTlr.ymDXzxt7.mNmOJ7P,4rOs","Token":"cillum sunt qui Lorem dolor"}]}')
         aioresponses.put(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.lock_booking(url=url_variant, **parameters)
-            assert normalize_result(put_booking_lock_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"Booking":{"ID":"http://yoMAnxJpiGEEkJWmzKnSqBtqhCnvIdMSr.cbrqcVvPcrHoB7.QLta4DcDk.jczRQZu-TfKCushfW+nJ6G0o2G1leLXCDu3a42jPisVbqbz","Time":{"Start":"1991-10-08T01:22:07.0Z","End":"2022-11-10T18:20:43.0Z"},"Devices":["https://xqNbClEPdpHKig.dhiiSiYrU3DYITw6tF1lmUdif8O07Y.LfqivCk3JNt7iUd9J,N4eDsNZfLZ70M","https://yTxELhUrJEDpBapgc.ttgsbLDKBsuj096crVKGCv,kj,hrV-RVDFyUhRLpwvGOaInHu1ZSt1drc5","http://urgvYKPgJ.wss5xn,ZSCgIP5RqnKMw5sFSj27mwK6wfLkBSkbnpwsw2hYZFqmdh+80zT-NM"],"Status":"active","You":false,"External":true,"Message":"Lorem ipsum incididunt","Type":"normal"},"Time":{"Start":"1983-04-17T07:30:29.0Z","End":"2022-12-07T12:03:19.0Z"},"Tokens":[{"Token":"ea Duis anim"},{"Device":"https://lujjGqZNTwEvcLV.nyfEzuMfcb,byZ1.XCuvg+T","Token":"consectetur aute nisi"},{"Device":"https://kFwUbbqqJHNFECezWeTvNmjTlr.ymDXzxt7.mNmOJ7P,4rOs","Token":"cillum sunt qui Lorem dolor"}]}')
         aioresponses.put(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.lock_booking(url=full_url, **parameters)
-            assert normalize_result(put_booking_lock_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.put(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.lock_booking(url=url, **parameters)
 
@@ -3773,41 +3824,43 @@
 @pytest.mark.asyncio
 async def test_list_devices(aioresponses: aioresponses):
     url = r'/devices'
     url_variant = r'devices'
     full_url = BASE_URL+r'/devices'
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"description":"occaecat ut non anim","owner":"http://XtyFMjWKLqVNOjoFVOCibGChfLnTd.elheA5xrKYP,KYInBcyGXAo7fWTRAFLv-I66+UEa11nOnUW,yrp7vU8tJDvqx-FBcm","url":"https://gUzGKHPeV.xtseja4ThHmONE6IMx"},{"description":"officia nisi ut","name":"ad amet dolore Duis","url":"https://xuSaiEaHtcvtcAzTVACnzItZUP.dpbsi.4CSbCelm2XPG6GJifZP5BwV","type":"cloud instantiable","owner":"http://knWGbtFvjEZogFuZq.jnbimyOtjLoxNnW04vVg+28XxLvtiBbTVsIXxMSxfV-cnpmwROVBavvKOxqv7Q"},{"description":"amet eu labore","url":"https://wrEF.iaf.vje-57RTm9JYGspOOJfsTdt0qLvKg914AbmBdlJfKZA4BFoJ","name":"sint cupidatat ipsum pariatur dolore","type":"device","owner":"http://NOdjkLvvuy.fihbxtyikUqV-5dwSkcBP+E4deORAAG2KGBsiq"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_devices(**parameters)
-            assert normalize_result(get_devices_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"description":"occaecat ut non anim","owner":"http://XtyFMjWKLqVNOjoFVOCibGChfLnTd.elheA5xrKYP,KYInBcyGXAo7fWTRAFLv-I66+UEa11nOnUW,yrp7vU8tJDvqx-FBcm","url":"https://gUzGKHPeV.xtseja4ThHmONE6IMx"},{"description":"officia nisi ut","name":"ad amet dolore Duis","url":"https://xuSaiEaHtcvtcAzTVACnzItZUP.dpbsi.4CSbCelm2XPG6GJifZP5BwV","type":"cloud instantiable","owner":"http://knWGbtFvjEZogFuZq.jnbimyOtjLoxNnW04vVg+28XxLvtiBbTVsIXxMSxfV-cnpmwROVBavvKOxqv7Q"},{"description":"amet eu labore","url":"https://wrEF.iaf.vje-57RTm9JYGspOOJfsTdt0qLvKg914AbmBdlJfKZA4BFoJ","name":"sint cupidatat ipsum pariatur dolore","type":"device","owner":"http://NOdjkLvvuy.fihbxtyikUqV-5dwSkcBP+E4deORAAG2KGBsiq"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_devices(url=url, **parameters)
-            assert normalize_result(get_devices_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"description":"occaecat ut non anim","owner":"http://XtyFMjWKLqVNOjoFVOCibGChfLnTd.elheA5xrKYP,KYInBcyGXAo7fWTRAFLv-I66+UEa11nOnUW,yrp7vU8tJDvqx-FBcm","url":"https://gUzGKHPeV.xtseja4ThHmONE6IMx"},{"description":"officia nisi ut","name":"ad amet dolore Duis","url":"https://xuSaiEaHtcvtcAzTVACnzItZUP.dpbsi.4CSbCelm2XPG6GJifZP5BwV","type":"cloud instantiable","owner":"http://knWGbtFvjEZogFuZq.jnbimyOtjLoxNnW04vVg+28XxLvtiBbTVsIXxMSxfV-cnpmwROVBavvKOxqv7Q"},{"description":"amet eu labore","url":"https://wrEF.iaf.vje-57RTm9JYGspOOJfsTdt0qLvKg914AbmBdlJfKZA4BFoJ","name":"sint cupidatat ipsum pariatur dolore","type":"device","owner":"http://NOdjkLvvuy.fihbxtyikUqV-5dwSkcBP+E4deORAAG2KGBsiq"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_devices(url=url_variant, **parameters)
-            assert normalize_result(get_devices_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"description":"occaecat ut non anim","owner":"http://XtyFMjWKLqVNOjoFVOCibGChfLnTd.elheA5xrKYP,KYInBcyGXAo7fWTRAFLv-I66+UEa11nOnUW,yrp7vU8tJDvqx-FBcm","url":"https://gUzGKHPeV.xtseja4ThHmONE6IMx"},{"description":"officia nisi ut","name":"ad amet dolore Duis","url":"https://xuSaiEaHtcvtcAzTVACnzItZUP.dpbsi.4CSbCelm2XPG6GJifZP5BwV","type":"cloud instantiable","owner":"http://knWGbtFvjEZogFuZq.jnbimyOtjLoxNnW04vVg+28XxLvtiBbTVsIXxMSxfV-cnpmwROVBavvKOxqv7Q"},{"description":"amet eu labore","url":"https://wrEF.iaf.vje-57RTm9JYGspOOJfsTdt0qLvKg914AbmBdlJfKZA4BFoJ","name":"sint cupidatat ipsum pariatur dolore","type":"device","owner":"http://NOdjkLvvuy.fihbxtyikUqV-5dwSkcBP+E4deORAAG2KGBsiq"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_devices(url=full_url, **parameters)
-            assert normalize_result(get_devices_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_devices(**parameters)
 
     for parameters in parameter_list:
@@ -3823,14 +3876,15 @@
                 resp = await client.list_devices(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_devices(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_devices(**parameters)
 
     for parameters in parameter_list:
@@ -3846,14 +3900,15 @@
                 resp = await client.list_devices(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_devices(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_devices(**parameters)
 
     for parameters in parameter_list:
@@ -3869,14 +3924,15 @@
                 resp = await client.list_devices(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_devices(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_devices(**parameters)
 
     for parameters in parameter_list:
@@ -3892,14 +3948,15 @@
                 resp = await client.list_devices(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_devices(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_devices(**parameters)
 
     for parameters in parameter_list:
@@ -3923,45 +3980,46 @@
 
 @pytest.mark.asyncio
 async def test_create_device(aioresponses: aioresponses):
     url = r'/devices'
     url_variant = r'devices'
     full_url = BASE_URL+r'/devices'
 
-    request_dict = json.loads(r'{"services":[],"url":"https://FFtBZqePJevWvqANceH.erzuirQaTbcwUTzpisvYDrbm0JMrsFw.-U1iS5kUOo","type":"device","connected":true,"owner":"https://mDCjpDPqCPPtDeHBrJuRtfOZdAkcLQgiM.kjDA0FCmSOocI6lV.q9RAXULVivUlme.Yb+A5VglKZF9jsM33IUv5MmtYkt4tbqo7-gGC4","description":"consequat id commodo","name":"amet Duis eiusmod dolor deserunt","experiment":"https://yZjFsGlZmXSOaJmchy.ezuSwTSEZ9RaYnbjr-R86Gm5bddW7BbgjWvaia3qfQMtJd,JFhTVyi7xYNvwoq.FegAtFIqvVB","announcedAvailability":[{"repeat":{"frequency":"DAILY","until":"1996-05-09T01:35:51.0Z"}}]}')
-    request = post_devices_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"services":[],"url":"https://FFtBZqePJevWvqANceH.erzuirQaTbcwUTzpisvYDrbm0JMrsFw.-U1iS5kUOo","type":"device","connected":true,"owner":"https://mDCjpDPqCPPtDeHBrJuRtfOZdAkcLQgiM.kjDA0FCmSOocI6lV.q9RAXULVivUlme.Yb+A5VglKZF9jsM33IUv5MmtYkt4tbqo7-gGC4","description":"consequat id commodo","name":"amet Duis eiusmod dolor deserunt","experiment":"https://yZjFsGlZmXSOaJmchy.ezuSwTSEZ9RaYnbjr-R86Gm5bddW7BbgjWvaia3qfQMtJd,JFhTVyi7xYNvwoq.FegAtFIqvVB","announcedAvailability":[{"repeat":{"frequency":"DAILY","until":"1996-05-09T01:35:51.0Z"}}]}')
 
     parameter_list = [{"changedUrl": "test_string", }, {}, ]
+
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_device(body=request, **parameters)
-            assert normalize_result(post_devices_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_device(url=url, body=request, **parameters)
-            assert normalize_result(post_devices_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_device(url=url_variant, body=request, **parameters)
-            assert normalize_result(post_devices_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_device(url=full_url, body=request, **parameters)
-            assert normalize_result(post_devices_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -3977,14 +4035,15 @@
                 resp = await client.create_device(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -4000,14 +4059,15 @@
                 resp = await client.create_device(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -4023,14 +4083,15 @@
                 resp = await client.create_device(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -4046,14 +4107,15 @@
                 resp = await client.create_device(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_device(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -4084,29 +4146,29 @@
     parameter_list = [{"flat_group": True, }, {}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_device(url=url, **parameters)
-            assert normalize_result(get_device_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_device(url=url_variant, **parameters)
-            assert normalize_result(get_device_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_device(url=full_url, **parameters)
-            assert normalize_result(get_device_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_device(url=url, **parameters)
 
@@ -4197,39 +4259,38 @@
 
 @pytest.mark.asyncio
 async def test_update_device(aioresponses: aioresponses):
     url = r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
-    request_dict = json.loads(r'{"services":[],"url":"https://FFtBZqePJevWvqANceH.erzuirQaTbcwUTzpisvYDrbm0JMrsFw.-U1iS5kUOo","type":"device","connected":true,"owner":"https://mDCjpDPqCPPtDeHBrJuRtfOZdAkcLQgiM.kjDA0FCmSOocI6lV.q9RAXULVivUlme.Yb+A5VglKZF9jsM33IUv5MmtYkt4tbqo7-gGC4","description":"consequat id commodo","name":"amet Duis eiusmod dolor deserunt","experiment":"https://yZjFsGlZmXSOaJmchy.ezuSwTSEZ9RaYnbjr-R86Gm5bddW7BbgjWvaia3qfQMtJd,JFhTVyi7xYNvwoq.FegAtFIqvVB","announcedAvailability":[{"repeat":{"frequency":"DAILY","until":"1996-05-09T01:35:51.0Z"}}]}')
-    request = patch_device_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"services":[],"url":"https://FFtBZqePJevWvqANceH.erzuirQaTbcwUTzpisvYDrbm0JMrsFw.-U1iS5kUOo","type":"device","connected":true,"owner":"https://mDCjpDPqCPPtDeHBrJuRtfOZdAkcLQgiM.kjDA0FCmSOocI6lV.q9RAXULVivUlme.Yb+A5VglKZF9jsM33IUv5MmtYkt4tbqo7-gGC4","description":"consequat id commodo","name":"amet Duis eiusmod dolor deserunt","experiment":"https://yZjFsGlZmXSOaJmchy.ezuSwTSEZ9RaYnbjr-R86Gm5bddW7BbgjWvaia3qfQMtJd,JFhTVyi7xYNvwoq.FegAtFIqvVB","announcedAvailability":[{"repeat":{"frequency":"DAILY","until":"1996-05-09T01:35:51.0Z"}}]}')
 
     parameter_list = [{"changedUrl": "test_string", }, {}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_device(url=url, body=request, **parameters)
-            assert normalize_result(patch_device_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_device(url=url_variant, body=request, **parameters)
-            assert normalize_result(patch_device_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"type":"device","owner":"http://wrvuppqewWdH.omhcAwZEk9qD7opUiXkFBrRItQoqFDF7XVlUNBNhMuyCMYhjfpg7qrt-Fj5hqnNkDvd8tzmY60V61j","url":"http://uFaodEpKyQkGvFI.gotilvYR.udrlbOB-hlPogvYKzKk","description":"fugiat eiusmod","name":"aute consequat veniam","services":[],"experiment":"http://RdmTyMiQYSUxtCuahvebSpQ.enR73CD5qG","connected":false}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_device(url=full_url, body=request, **parameters)
-            assert normalize_result(patch_device_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_device(url=url, body=request, **parameters)
 
@@ -4441,29 +4502,29 @@
     parameter_list = [{"changedUrl": "test_string", }, {}, ]
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"instance":{"announcedAvailability":[{"start":"1955-04-07T01:22:58.0Z","end":"1995-07-10T11:59:14.0Z"},{"end":"2006-05-22T14:58:01.0Z","start":"1956-06-29T18:16:35.0Z"},{"end":"2013-11-28T07:03:49.0Z"},{"end":"2015-04-21T18:19:04.0Z","start":"1975-07-14T08:16:38.0Z"}],"url":"http://uqyLriKDNyKa.qeZcaJtVX9mfvD76xUF+W4nYYFiXhN--1QmKZdxJnnq","services":[],"type":"device","connected":true,"name":"in","owner":"http://XtPxmagFFBylFzvNnkgMTYi.yvmlIqZeAORZPbJktCdGBIj2aFx5zB","description":"nostrud Lorem commodo Excepteur","experiment":"http://ziGqQoyUsaiCVXWUsGq.vgYEjjfQYlaoNU0.TNshwmZX97ESZapPxeXRR6oyHetq"},"deviceToken":"irure eu"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.instantiate_device(url=url, **parameters)
-            assert normalize_result(post_device_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"instance":{"announcedAvailability":[{"start":"1955-04-07T01:22:58.0Z","end":"1995-07-10T11:59:14.0Z"},{"end":"2006-05-22T14:58:01.0Z","start":"1956-06-29T18:16:35.0Z"},{"end":"2013-11-28T07:03:49.0Z"},{"end":"2015-04-21T18:19:04.0Z","start":"1975-07-14T08:16:38.0Z"}],"url":"http://uqyLriKDNyKa.qeZcaJtVX9mfvD76xUF+W4nYYFiXhN--1QmKZdxJnnq","services":[],"type":"device","connected":true,"name":"in","owner":"http://XtPxmagFFBylFzvNnkgMTYi.yvmlIqZeAORZPbJktCdGBIj2aFx5zB","description":"nostrud Lorem commodo Excepteur","experiment":"http://ziGqQoyUsaiCVXWUsGq.vgYEjjfQYlaoNU0.TNshwmZX97ESZapPxeXRR6oyHetq"},"deviceToken":"irure eu"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.instantiate_device(url=url_variant, **parameters)
-            assert normalize_result(post_device_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"instance":{"announcedAvailability":[{"start":"1955-04-07T01:22:58.0Z","end":"1995-07-10T11:59:14.0Z"},{"end":"2006-05-22T14:58:01.0Z","start":"1956-06-29T18:16:35.0Z"},{"end":"2013-11-28T07:03:49.0Z"},{"end":"2015-04-21T18:19:04.0Z","start":"1975-07-14T08:16:38.0Z"}],"url":"http://uqyLriKDNyKa.qeZcaJtVX9mfvD76xUF+W4nYYFiXhN--1QmKZdxJnnq","services":[],"type":"device","connected":true,"name":"in","owner":"http://XtPxmagFFBylFzvNnkgMTYi.yvmlIqZeAORZPbJktCdGBIj2aFx5zB","description":"nostrud Lorem commodo Excepteur","experiment":"http://ziGqQoyUsaiCVXWUsGq.vgYEjjfQYlaoNU0.TNshwmZX97ESZapPxeXRR6oyHetq"},"deviceToken":"irure eu"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.instantiate_device(url=full_url, **parameters)
-            assert normalize_result(post_device_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.instantiate_device(url=url, **parameters)
 
@@ -4554,39 +4615,38 @@
 
 @pytest.mark.asyncio
 async def test_add_availability_rules(aioresponses: aioresponses):
     url = r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/availability'
     url_variant = r'devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/availability'
     full_url = BASE_URL+r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/availability'
 
-    request_dict = json.loads(r'[{"start":"1976-10-07T22:53:32.0Z","end":"2021-01-23T10:58:58.0Z","available":true,"repeat":{"until":"1999-07-02T02:45:39.0Z"}},{"end":"1987-01-05T01:08:15.0Z"}]')
-    request = post_device_availability_request_body_write_from_dict(request_dict)
+    request = json.loads(r'[{"start":"1976-10-07T22:53:32.0Z","end":"2021-01-23T10:58:58.0Z","available":true,"repeat":{"until":"1999-07-02T02:45:39.0Z"}},{"end":"1987-01-05T01:08:15.0Z"}]')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"end":"1992-10-14T09:14:27.0Z"},{"start":"1978-02-16T19:07:22.0Z","end":"2008-06-15T01:24:43.0Z"},{"end":"1972-02-03T10:17:33.0Z"},{"start":"1973-01-02T03:15:47.0Z","end":"1987-10-14T09:42:59.0Z"},{"end":"1980-02-28T18:27:09.0Z","start":"1991-04-19T08:25:57.0Z"}]')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.add_availability_rules(url=url, body=request, **parameters)
-            assert normalize_result(post_device_availability_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"end":"1992-10-14T09:14:27.0Z"},{"start":"1978-02-16T19:07:22.0Z","end":"2008-06-15T01:24:43.0Z"},{"end":"1972-02-03T10:17:33.0Z"},{"start":"1973-01-02T03:15:47.0Z","end":"1987-10-14T09:42:59.0Z"},{"end":"1980-02-28T18:27:09.0Z","start":"1991-04-19T08:25:57.0Z"}]')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.add_availability_rules(url=url_variant, body=request, **parameters)
-            assert normalize_result(post_device_availability_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"end":"1992-10-14T09:14:27.0Z"},{"start":"1978-02-16T19:07:22.0Z","end":"2008-06-15T01:24:43.0Z"},{"end":"1972-02-03T10:17:33.0Z"},{"start":"1973-01-02T03:15:47.0Z","end":"1987-10-14T09:42:59.0Z"},{"end":"1980-02-28T18:27:09.0Z","start":"1991-04-19T08:25:57.0Z"}]')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.add_availability_rules(url=full_url, body=request, **parameters)
-            assert normalize_result(post_device_availability_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.add_availability_rules(url=url, body=request, **parameters)
 
@@ -4684,29 +4744,29 @@
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'"consectetur in do nisi"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_websocket_token(url=url, **parameters)
-            assert normalize_result(post_device_websocket_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'"consectetur in do nisi"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_websocket_token(url=url_variant, **parameters)
-            assert normalize_result(post_device_websocket_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'"consectetur in do nisi"')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_websocket_token(url=full_url, **parameters)
-            assert normalize_result(post_device_websocket_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_websocket_token(url=url, **parameters)
 
@@ -4797,16 +4857,15 @@
 
 @pytest.mark.asyncio
 async def test_send_signaling_message(aioresponses: aioresponses):
     url = r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/signaling'
     url_variant = r'devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/signaling'
     full_url = BASE_URL+r'/devices/c799cc2e-cdc5-4143-973a-6f56a5afa82c/signaling'
 
-    request_dict = json.loads(r'{"messageType":"command","command":"createPeerconnection","connectionType":"websocket","connectionUrl":"http://mSxcAxcNBEEObpLmSlWMbhgcDFFq.phuibR+NAH9qR2hG,VoGNZCgZKXd5f-JF","services":[{"serviceType":"https://WN.yyqil0X0kH-nSbucxHwUKTp6riWuOEsxSyNTZz","serviceId":"ad reprehenderit","remoteServiceId":"laborum velit"},{"serviceType":"https://GaxqG.fcVGX0FK","serviceId":"exercitation","remoteServiceId":"dolor magna in proident"}],"tiebreaker":true,"config":{}}')
-    request = post_device_signaling_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"messageType":"command","command":"createPeerconnection","connectionType":"websocket","connectionUrl":"http://mSxcAxcNBEEObpLmSlWMbhgcDFFq.phuibR+NAH9qR2hG,VoGNZCgZKXd5f-JF","services":[{"serviceType":"https://WN.yyqil0X0kH-nSbucxHwUKTp6riWuOEsxSyNTZz","serviceId":"ad reprehenderit","remoteServiceId":"laborum velit"},{"serviceType":"https://GaxqG.fcVGX0FK","serviceId":"exercitation","remoteServiceId":"dolor magna in proident"}],"tiebreaker":true,"config":{}}')
 
     parameter_list = [{"peerconnection_url": "test_string", }, ]
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200)
         async with APIClient(BASE_URL) as client:
             resp = await client.send_signaling_message(url=url, body=request, **parameters)
@@ -4915,41 +4974,43 @@
 @pytest.mark.asyncio
 async def test_list_peerconnections(aioresponses: aioresponses):
     url = r'/peerconnections'
     url_variant = r'peerconnections'
     full_url = BASE_URL+r'/peerconnections'
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"devices":[{"url":"https://AcAm.lbXLj6e"},{"url":"http://XrTgiHePnXvRPczPBULvYtI.wsavVsuGOEjKj7O3CmZC3P2wKB4,hn4VXd6cXxcgqpSF9gDwinLCTPN0xjFVloE.mcO9"}],"url":"https://HdGqlUwYyIraClLraHacgbNvWINA.clJ3KvdUzu2GNj4hKj,RdgY6seg"},{"devices":[{"url":"https://iIRIvlwbF.obmg.EeycdcbdoSy62ARR1HP7BQpX"},{"url":"https://XnJbyygWStGohyNKERsjdkm.urE4I2GeltAe-"}]}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_peerconnections(**parameters)
-            assert normalize_result(get_peerconnections_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"devices":[{"url":"https://AcAm.lbXLj6e"},{"url":"http://XrTgiHePnXvRPczPBULvYtI.wsavVsuGOEjKj7O3CmZC3P2wKB4,hn4VXd6cXxcgqpSF9gDwinLCTPN0xjFVloE.mcO9"}],"url":"https://HdGqlUwYyIraClLraHacgbNvWINA.clJ3KvdUzu2GNj4hKj,RdgY6seg"},{"devices":[{"url":"https://iIRIvlwbF.obmg.EeycdcbdoSy62ARR1HP7BQpX"},{"url":"https://XnJbyygWStGohyNKERsjdkm.urE4I2GeltAe-"}]}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_peerconnections(url=url, **parameters)
-            assert normalize_result(get_peerconnections_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"devices":[{"url":"https://AcAm.lbXLj6e"},{"url":"http://XrTgiHePnXvRPczPBULvYtI.wsavVsuGOEjKj7O3CmZC3P2wKB4,hn4VXd6cXxcgqpSF9gDwinLCTPN0xjFVloE.mcO9"}],"url":"https://HdGqlUwYyIraClLraHacgbNvWINA.clJ3KvdUzu2GNj4hKj,RdgY6seg"},{"devices":[{"url":"https://iIRIvlwbF.obmg.EeycdcbdoSy62ARR1HP7BQpX"},{"url":"https://XnJbyygWStGohyNKERsjdkm.urE4I2GeltAe-"}]}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_peerconnections(url=url_variant, **parameters)
-            assert normalize_result(get_peerconnections_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"devices":[{"url":"https://AcAm.lbXLj6e"},{"url":"http://XrTgiHePnXvRPczPBULvYtI.wsavVsuGOEjKj7O3CmZC3P2wKB4,hn4VXd6cXxcgqpSF9gDwinLCTPN0xjFVloE.mcO9"}],"url":"https://HdGqlUwYyIraClLraHacgbNvWINA.clJ3KvdUzu2GNj4hKj,RdgY6seg"},{"devices":[{"url":"https://iIRIvlwbF.obmg.EeycdcbdoSy62ARR1HP7BQpX"},{"url":"https://XnJbyygWStGohyNKERsjdkm.urE4I2GeltAe-"}]}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_peerconnections(url=full_url, **parameters)
-            assert normalize_result(get_peerconnections_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_peerconnections(**parameters)
 
     for parameters in parameter_list:
@@ -4965,14 +5026,15 @@
                 resp = await client.list_peerconnections(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_peerconnections(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_peerconnections(**parameters)
 
     for parameters in parameter_list:
@@ -4988,14 +5050,15 @@
                 resp = await client.list_peerconnections(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_peerconnections(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_peerconnections(**parameters)
 
     for parameters in parameter_list:
@@ -5011,14 +5074,15 @@
                 resp = await client.list_peerconnections(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_peerconnections(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_peerconnections(**parameters)
 
     for parameters in parameter_list:
@@ -5034,14 +5098,15 @@
                 resp = await client.list_peerconnections(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_peerconnections(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_peerconnections(**parameters)
 
     for parameters in parameter_list:
@@ -5065,72 +5130,74 @@
 
 @pytest.mark.asyncio
 async def test_create_peerconnection(aioresponses: aioresponses):
     url = r'/peerconnections'
     url_variant = r'peerconnections'
     full_url = BASE_URL+r'/peerconnections'
 
-    request_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
-    request = post_peerconnections_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
 
     parameter_list = [{"closedUrl": "test_string", "statusChangedUrl": "test_string", }, {"statusChangedUrl": "test_string", }, {"closedUrl": "test_string", }, {}, ]
+
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(body=request, **parameters)
-            assert normalize_result(post_peerconnections_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(url=url, body=request, **parameters)
-            assert normalize_result(post_peerconnections_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(url=url_variant, body=request, **parameters)
-            assert normalize_result(post_peerconnections_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(url=full_url, body=request, **parameters)
-            assert normalize_result(post_peerconnections_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
+
     for parameters in parameter_list:
         response_202_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(body=request, **parameters)
-            assert normalize_result(post_peerconnections_response_body202_read_to_dict(resp)) == normalize_result(response_202_dict)
+            assert normalize_result(resp) == normalize_result(response_202_dict)
 
     for parameters in parameter_list:
         response_202_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(url=url, body=request, **parameters)
-            assert normalize_result(post_peerconnections_response_body202_read_to_dict(resp)) == normalize_result(response_202_dict)
+            assert normalize_result(resp) == normalize_result(response_202_dict)
 
     for parameters in parameter_list:
         response_202_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(url=url_variant, body=request, **parameters)
-            assert normalize_result(post_peerconnections_response_body202_read_to_dict(resp)) == normalize_result(response_202_dict)
+            assert normalize_result(resp) == normalize_result(response_202_dict)
 
     for parameters in parameter_list:
         response_202_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_peerconnection(url=full_url, body=request, **parameters)
-            assert normalize_result(post_peerconnections_response_body202_read_to_dict(resp)) == normalize_result(response_202_dict)
+            assert normalize_result(resp) == normalize_result(response_202_dict)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_peerconnection(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -5146,14 +5213,15 @@
                 resp = await client.create_peerconnection(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_peerconnection(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_peerconnection(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -5169,14 +5237,15 @@
                 resp = await client.create_peerconnection(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_peerconnection(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_peerconnection(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -5192,14 +5261,15 @@
                 resp = await client.create_peerconnection(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_peerconnection(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_peerconnection(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -5215,14 +5285,15 @@
                 resp = await client.create_peerconnection(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_peerconnection(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_peerconnection(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -5253,29 +5324,29 @@
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_peerconnection(url=url, **parameters)
-            assert normalize_result(get_peerconnection_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_peerconnection(url=url_variant, **parameters)
-            assert normalize_result(get_peerconnection_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"devices":[{"config":{"services":[{"remoteServiceId":"aliquip cillum sit laboris proident","serviceType":"http://KQNKmkiBeAKZTYtYeKBfWScV.lrytkFxV,ZrP-XBrNY-Pt"},{"remoteServiceId":"non aliqua proident","serviceType":"https://WnrvOdiQDOMpdYMcTq.noO+WfcTGn-SJlF,gLZ.+0sd4lfOBqeRcm0VW3vdF-s5","serviceId":"occaecat"},{"serviceType":"http://ZoSEaDhJkgXvaseY.myrzUuSpBSXiaGe4n-+KHudVEZQfvK3O+nRIwYJTSE5Ny,L","serviceId":"laboris"},{"serviceType":"https://GkopJXScAvTsPblHOnULiGlmEmOkeEn.uwbJBdQI"}]}}],"status":"failed","url":"https://bMJFHTrmqHvixazrXAYqbQYHMSCMKO.yjkNKx6ocxMqy"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_peerconnection(url=full_url, **parameters)
-            assert normalize_result(get_peerconnection_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_peerconnection(url=url, **parameters)
 
@@ -5481,41 +5552,43 @@
 @pytest.mark.asyncio
 async def test_list_experiments(aioresponses: aioresponses):
     url = r'/experiments'
     url_variant = r'experiments'
     full_url = BASE_URL+r'/experiments'
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{},{"status":"finished","url":"https://BhyolnlHwo.vigvwYRXrGvTctinm4bD6mAFEB,G3GjZbm3PIA7Ol+JNMUumyt0"},{"status":"finished","url":"https://gsYIkbvdZLBXqpwanqbvKdHppdZrdHY.snGgXKR.n+A6zyeKl2ZHX"},{"url":"https://oYvRCkEjCOExundq.qbzih9w3Q8CUKWCMEoNeMO79mu4r","status":"running"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_experiments(**parameters)
-            assert normalize_result(get_experiments_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{},{"status":"finished","url":"https://BhyolnlHwo.vigvwYRXrGvTctinm4bD6mAFEB,G3GjZbm3PIA7Ol+JNMUumyt0"},{"status":"finished","url":"https://gsYIkbvdZLBXqpwanqbvKdHppdZrdHY.snGgXKR.n+A6zyeKl2ZHX"},{"url":"https://oYvRCkEjCOExundq.qbzih9w3Q8CUKWCMEoNeMO79mu4r","status":"running"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_experiments(url=url, **parameters)
-            assert normalize_result(get_experiments_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{},{"status":"finished","url":"https://BhyolnlHwo.vigvwYRXrGvTctinm4bD6mAFEB,G3GjZbm3PIA7Ol+JNMUumyt0"},{"status":"finished","url":"https://gsYIkbvdZLBXqpwanqbvKdHppdZrdHY.snGgXKR.n+A6zyeKl2ZHX"},{"url":"https://oYvRCkEjCOExundq.qbzih9w3Q8CUKWCMEoNeMO79mu4r","status":"running"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_experiments(url=url_variant, **parameters)
-            assert normalize_result(get_experiments_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{},{"status":"finished","url":"https://BhyolnlHwo.vigvwYRXrGvTctinm4bD6mAFEB,G3GjZbm3PIA7Ol+JNMUumyt0"},{"status":"finished","url":"https://gsYIkbvdZLBXqpwanqbvKdHppdZrdHY.snGgXKR.n+A6zyeKl2ZHX"},{"url":"https://oYvRCkEjCOExundq.qbzih9w3Q8CUKWCMEoNeMO79mu4r","status":"running"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_experiments(url=full_url, **parameters)
-            assert normalize_result(get_experiments_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_experiments(**parameters)
 
     for parameters in parameter_list:
@@ -5531,14 +5604,15 @@
                 resp = await client.list_experiments(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_experiments(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_experiments(**parameters)
 
     for parameters in parameter_list:
@@ -5554,14 +5628,15 @@
                 resp = await client.list_experiments(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_experiments(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_experiments(**parameters)
 
     for parameters in parameter_list:
@@ -5577,14 +5652,15 @@
                 resp = await client.list_experiments(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_experiments(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_experiments(**parameters)
 
     for parameters in parameter_list:
@@ -5600,14 +5676,15 @@
                 resp = await client.list_experiments(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_experiments(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_experiments(**parameters)
 
     for parameters in parameter_list:
@@ -5631,72 +5708,74 @@
 
 @pytest.mark.asyncio
 async def test_create_experiment(aioresponses: aioresponses):
     url = r'/experiments'
     url_variant = r'experiments'
     full_url = BASE_URL+r'/experiments'
 
-    request_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
-    request = post_experiments_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_experiment(body=request, **parameters)
-            assert normalize_result(post_experiments_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_experiment(url=url, body=request, **parameters)
-            assert normalize_result(post_experiments_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_experiment(url=url_variant, body=request, **parameters)
-            assert normalize_result(post_experiments_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_experiment(url=full_url, body=request, **parameters)
-            assert normalize_result(post_experiments_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
+
     for parameters in parameter_list:
         response_202_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_experiment(body=request, **parameters)
-            assert normalize_result(post_experiments_response_body202_read_to_dict(resp)) == normalize_result(response_202_dict)
+            assert normalize_result(resp) == normalize_result(response_202_dict)
 
     for parameters in parameter_list:
         response_202_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_experiment(url=url, body=request, **parameters)
-            assert normalize_result(post_experiments_response_body202_read_to_dict(resp)) == normalize_result(response_202_dict)
+            assert normalize_result(resp) == normalize_result(response_202_dict)
 
     for parameters in parameter_list:
         response_202_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_experiment(url=url_variant, body=request, **parameters)
-            assert normalize_result(post_experiments_response_body202_read_to_dict(resp)) == normalize_result(response_202_dict)
+            assert normalize_result(resp) == normalize_result(response_202_dict)
 
     for parameters in parameter_list:
         response_202_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_experiment(url=full_url, body=request, **parameters)
-            assert normalize_result(post_experiments_response_body202_read_to_dict(resp)) == normalize_result(response_202_dict)
+            assert normalize_result(resp) == normalize_result(response_202_dict)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_experiment(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -5712,14 +5791,15 @@
                 resp = await client.create_experiment(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_experiment(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_experiment(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -5735,14 +5815,15 @@
                 resp = await client.create_experiment(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_experiment(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_experiment(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -5758,14 +5839,15 @@
                 resp = await client.create_experiment(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_experiment(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_experiment(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -5781,14 +5863,15 @@
                 resp = await client.create_experiment(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_experiment(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_experiment(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -5819,29 +5902,29 @@
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_experiment(url=url, **parameters)
-            assert normalize_result(get_experiment_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_experiment(url=url_variant, **parameters)
-            assert normalize_result(get_experiment_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_experiment(url=full_url, **parameters)
-            assert normalize_result(get_experiment_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_experiment(url=url, **parameters)
 
@@ -5932,60 +6015,59 @@
 
 @pytest.mark.asyncio
 async def test_update_experiment(aioresponses: aioresponses):
     url = r'/experiments/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'experiments/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/experiments/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
-    request_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
-    request = patch_experiment_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
 
     parameter_list = [{"changedURL": "test_string", }, {}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_experiment(url=url, body=request, **parameters)
-            assert normalize_result(patch_experiment_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_experiment(url=url_variant, body=request, **parameters)
-            assert normalize_result(patch_experiment_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_experiment(url=full_url, body=request, **parameters)
-            assert normalize_result(patch_experiment_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_202_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_experiment(url=url, body=request, **parameters)
-            assert normalize_result(patch_experiment_response_body202_read_to_dict(resp)) == normalize_result(response_202_dict)
+            assert normalize_result(resp) == normalize_result(response_202_dict)
 
     for parameters in parameter_list:
         response_202_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_experiment(url=url_variant, body=request, **parameters)
-            assert normalize_result(patch_experiment_response_body202_read_to_dict(resp)) == normalize_result(response_202_dict)
+            assert normalize_result(resp) == normalize_result(response_202_dict)
 
     for parameters in parameter_list:
         response_202_dict = json.loads(r'{"serviceConfigurations":[{"serviceType":"https://IXZOfMP.rzhvMvg4iLrkdXyhDeA9H4pqmcpRj3O265bh5nvxd9FDN45pLu4K2drZRE","participants":[{"role":"culpa","serviceId":"magna mollit culpa ullamco"},{"serviceId":"sint exercitation","role":"ipsum quis eu Duis"},{"serviceId":"ut","role":"fugiat ad nisi"},{"role":"magna","serviceId":"sint labore adipisicing irure"}]},{"participants":[{"role":"id consectetur","serviceId":"et in Duis ex"},{"serviceId":"elit ex","role":"exercitation officia"},{"role":"cillum"},{"role":"enim","serviceId":"eiusmod in exercitation dolor"}],"serviceType":"http://umRRzhl.sfgzT1DQ3Tj2m2zEhAY76w9dG,4G6nky6OFWCkt8HlCEsQ"},{"serviceType":"https://otLDMGJmSIZCDLKFdMtjUIklvxIZxKUG.pghtJNv9Viw18dTP","participants":[]}],"status":"running","url":"https://OtfusAGhcySWtkDDwg.usEkzpi3QbivBEGBU4kK1fUNf8ePt1T1Ga6ZT","bookingTime":{"startTime":"2014-12-23T04:32:46.0Z"},"roles":[{"name":"in minim incididunt"},{"name":"ut deserunt","description":"amet in in"},{"description":"Ut","name":"culpa ut nulla"}]}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=202, payload=response_202_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_experiment(url=full_url, body=request, **parameters)
-            assert normalize_result(patch_experiment_response_body202_read_to_dict(resp)) == normalize_result(response_202_dict)
+            assert normalize_result(resp) == normalize_result(response_202_dict)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_experiment(url=url, body=request, **parameters)
 
@@ -6191,41 +6273,43 @@
 @pytest.mark.asyncio
 async def test_list_institutions(aioresponses: aioresponses):
     url = r'/institutions'
     url_variant = r'institutions'
     full_url = BASE_URL+r'/institutions'
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"apiToken":"in","homepage":"http://AD.srkrwnE","federatedApi":"https://biGcjlhbXIfU.fobmMh5kJdzqTQTq,+,5NFaaHwy","name":"laboris quis laborum nostrud","api":"https://lmwVKpUfU.qmZ5NXKtqrvyDDhPi6J,,vVOl2-hR+Kf694QBp.CZ"},{"apiToken":"voluptate enim mollit dolore reprehenderit","name":"ut qui quis","federatedApi":"http://dDsLV.zalLjx-X7AMbA0k,LJFvo4lCNtMopJ0hh5DJspMxmoLkHl5a","api":"https://FTkfIDuZXcsKUwVx.ceNT3kiETNdewalDCrYwNRv5loWq2","homepage":"http://aaNvNuixGVmKFHADrqIGBlguqQIu.annhUqRD"},{"name":"aliquip","homepage":"https://vQoOZjOxsUkLpmtBvSh.nusbvrXkK"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_institutions(**parameters)
-            assert normalize_result(get_institutions_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"apiToken":"in","homepage":"http://AD.srkrwnE","federatedApi":"https://biGcjlhbXIfU.fobmMh5kJdzqTQTq,+,5NFaaHwy","name":"laboris quis laborum nostrud","api":"https://lmwVKpUfU.qmZ5NXKtqrvyDDhPi6J,,vVOl2-hR+Kf694QBp.CZ"},{"apiToken":"voluptate enim mollit dolore reprehenderit","name":"ut qui quis","federatedApi":"http://dDsLV.zalLjx-X7AMbA0k,LJFvo4lCNtMopJ0hh5DJspMxmoLkHl5a","api":"https://FTkfIDuZXcsKUwVx.ceNT3kiETNdewalDCrYwNRv5loWq2","homepage":"http://aaNvNuixGVmKFHADrqIGBlguqQIu.annhUqRD"},{"name":"aliquip","homepage":"https://vQoOZjOxsUkLpmtBvSh.nusbvrXkK"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_institutions(url=url, **parameters)
-            assert normalize_result(get_institutions_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"apiToken":"in","homepage":"http://AD.srkrwnE","federatedApi":"https://biGcjlhbXIfU.fobmMh5kJdzqTQTq,+,5NFaaHwy","name":"laboris quis laborum nostrud","api":"https://lmwVKpUfU.qmZ5NXKtqrvyDDhPi6J,,vVOl2-hR+Kf694QBp.CZ"},{"apiToken":"voluptate enim mollit dolore reprehenderit","name":"ut qui quis","federatedApi":"http://dDsLV.zalLjx-X7AMbA0k,LJFvo4lCNtMopJ0hh5DJspMxmoLkHl5a","api":"https://FTkfIDuZXcsKUwVx.ceNT3kiETNdewalDCrYwNRv5loWq2","homepage":"http://aaNvNuixGVmKFHADrqIGBlguqQIu.annhUqRD"},{"name":"aliquip","homepage":"https://vQoOZjOxsUkLpmtBvSh.nusbvrXkK"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_institutions(url=url_variant, **parameters)
-            assert normalize_result(get_institutions_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'[{"apiToken":"in","homepage":"http://AD.srkrwnE","federatedApi":"https://biGcjlhbXIfU.fobmMh5kJdzqTQTq,+,5NFaaHwy","name":"laboris quis laborum nostrud","api":"https://lmwVKpUfU.qmZ5NXKtqrvyDDhPi6J,,vVOl2-hR+Kf694QBp.CZ"},{"apiToken":"voluptate enim mollit dolore reprehenderit","name":"ut qui quis","federatedApi":"http://dDsLV.zalLjx-X7AMbA0k,LJFvo4lCNtMopJ0hh5DJspMxmoLkHl5a","api":"https://FTkfIDuZXcsKUwVx.ceNT3kiETNdewalDCrYwNRv5loWq2","homepage":"http://aaNvNuixGVmKFHADrqIGBlguqQIu.annhUqRD"},{"name":"aliquip","homepage":"https://vQoOZjOxsUkLpmtBvSh.nusbvrXkK"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_institutions(url=full_url, **parameters)
-            assert normalize_result(get_institutions_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_institutions(**parameters)
 
     for parameters in parameter_list:
@@ -6241,14 +6325,15 @@
                 resp = await client.list_institutions(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_institutions(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_institutions(**parameters)
 
     for parameters in parameter_list:
@@ -6264,14 +6349,15 @@
                 resp = await client.list_institutions(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_institutions(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_institutions(**parameters)
 
     for parameters in parameter_list:
@@ -6287,14 +6373,15 @@
                 resp = await client.list_institutions(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_institutions(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_institutions(**parameters)
 
     for parameters in parameter_list:
@@ -6310,14 +6397,15 @@
                 resp = await client.list_institutions(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_institutions(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_institutions(**parameters)
 
     for parameters in parameter_list:
@@ -6341,45 +6429,46 @@
 
 @pytest.mark.asyncio
 async def test_create_institution(aioresponses: aioresponses):
     url = r'/institutions'
     url_variant = r'institutions'
     full_url = BASE_URL+r'/institutions'
 
-    request_dict = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
-    request = post_institutions_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_institution(body=request, **parameters)
-            assert normalize_result(post_institutions_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_institution(url=url, body=request, **parameters)
-            assert normalize_result(post_institutions_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_institution(url=url_variant, body=request, **parameters)
-            assert normalize_result(post_institutions_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
         response_201_dict = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_institution(url=full_url, body=request, **parameters)
-            assert normalize_result(post_institutions_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_institution(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -6395,14 +6484,15 @@
                 resp = await client.create_institution(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_institution(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_institution(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -6418,14 +6508,15 @@
                 resp = await client.create_institution(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_institution(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_institution(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -6441,14 +6532,15 @@
                 resp = await client.create_institution(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_institution(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_institution(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -6464,14 +6556,15 @@
                 resp = await client.create_institution(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_institution(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_institution(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -6502,29 +6595,29 @@
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_institution(url=url, **parameters)
-            assert normalize_result(get_institution_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_institution(url=url_variant, **parameters)
-            assert normalize_result(get_institution_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.get_institution(url=full_url, **parameters)
-            assert normalize_result(get_institution_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.get_institution(url=url, **parameters)
 
@@ -6615,39 +6708,38 @@
 
 @pytest.mark.asyncio
 async def test_update_institution(aioresponses: aioresponses):
     url = r'/institutions/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'institutions/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/institutions/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
-    request_dict = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
-    request = patch_institution_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_institution(url=url, body=request, **parameters)
-            assert normalize_result(patch_institution_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_institution(url=url_variant, body=request, **parameters)
-            assert normalize_result(patch_institution_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         response_200_dict = json.loads(r'{"apiToken":"magna","homepage":"http://dnHzghTNxuBrmqAWZv.fwhbkLyXjhTbPAPq,q.G2UiIeLAil4SFtxYpK","federatedApi":"http://OctPepLeLlhbGXRDmOjZUiaXvkFfg.tugbAFLU.k4TvtlGrpw","api":"http://h.tefFdL9KZgYjwLl,9RGFYTdC88cnq6EKQCGH4ZyYkM6b","name":"eu dolor"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.update_institution(url=full_url, body=request, **parameters)
-            assert normalize_result(patch_institution_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.update_institution(url=url, body=request, **parameters)
 
@@ -6853,41 +6945,43 @@
 @pytest.mark.asyncio
 async def test_list_updates(aioresponses: aioresponses):
     url = r'/updates'
     url_variant = r'updates'
     full_url = BASE_URL+r'/updates'
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"device_id":"amet proident","latest_version":"sunt","latest_version_link":"http://PFzkKlx.ikRP2N+CI-nv-GYdvXXiO,ngMrQev"}]')
+        response_200_dict = json.loads(r'[{"device_id":"laboris id esse voluptate","latest_version":"consectetur dolore eiusmod irure Ut","latest_version_link":"http://yDIRQywQVj.itoplrH.5.ZvDoQAWF,+mygysRlPEudD4CAcFtfH9T0nhlJ6Xs"},{"device_id":"ad sed in sit","latest_version":"do","latest_version_link":"https://ewOyOPLCYvOABMcIGaCT.wdbr+"},{"device_id":"commodo culpa non","latest_version":"commodo","latest_version_link":"https://qCFBSmpDECUttVJHEYqhktwLjsTJYA.enjwytNETkqFXbq9hn+bSYQ4qZDe+bGKYIm9.qQm07sEa4PKCM4uVmzNuDK4QWej"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_updates(**parameters)
-            assert normalize_result(get_updates_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"device_id":"amet proident","latest_version":"sunt","latest_version_link":"http://PFzkKlx.ikRP2N+CI-nv-GYdvXXiO,ngMrQev"}]')
+        response_200_dict = json.loads(r'[{"device_id":"laboris id esse voluptate","latest_version":"consectetur dolore eiusmod irure Ut","latest_version_link":"http://yDIRQywQVj.itoplrH.5.ZvDoQAWF,+mygysRlPEudD4CAcFtfH9T0nhlJ6Xs"},{"device_id":"ad sed in sit","latest_version":"do","latest_version_link":"https://ewOyOPLCYvOABMcIGaCT.wdbr+"},{"device_id":"commodo culpa non","latest_version":"commodo","latest_version_link":"https://qCFBSmpDECUttVJHEYqhktwLjsTJYA.enjwytNETkqFXbq9hn+bSYQ4qZDe+bGKYIm9.qQm07sEa4PKCM4uVmzNuDK4QWej"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_updates(url=url, **parameters)
-            assert normalize_result(get_updates_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"device_id":"amet proident","latest_version":"sunt","latest_version_link":"http://PFzkKlx.ikRP2N+CI-nv-GYdvXXiO,ngMrQev"}]')
+        response_200_dict = json.loads(r'[{"device_id":"laboris id esse voluptate","latest_version":"consectetur dolore eiusmod irure Ut","latest_version_link":"http://yDIRQywQVj.itoplrH.5.ZvDoQAWF,+mygysRlPEudD4CAcFtfH9T0nhlJ6Xs"},{"device_id":"ad sed in sit","latest_version":"do","latest_version_link":"https://ewOyOPLCYvOABMcIGaCT.wdbr+"},{"device_id":"commodo culpa non","latest_version":"commodo","latest_version_link":"https://qCFBSmpDECUttVJHEYqhktwLjsTJYA.enjwytNETkqFXbq9hn+bSYQ4qZDe+bGKYIm9.qQm07sEa4PKCM4uVmzNuDK4QWej"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_updates(url=url_variant, **parameters)
-            assert normalize_result(get_updates_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'[{"device_id":"amet proident","latest_version":"sunt","latest_version_link":"http://PFzkKlx.ikRP2N+CI-nv-GYdvXXiO,ngMrQev"}]')
+        response_200_dict = json.loads(r'[{"device_id":"laboris id esse voluptate","latest_version":"consectetur dolore eiusmod irure Ut","latest_version_link":"http://yDIRQywQVj.itoplrH.5.ZvDoQAWF,+mygysRlPEudD4CAcFtfH9T0nhlJ6Xs"},{"device_id":"ad sed in sit","latest_version":"do","latest_version_link":"https://ewOyOPLCYvOABMcIGaCT.wdbr+"},{"device_id":"commodo culpa non","latest_version":"commodo","latest_version_link":"https://qCFBSmpDECUttVJHEYqhktwLjsTJYA.enjwytNETkqFXbq9hn+bSYQ4qZDe+bGKYIm9.qQm07sEa4PKCM4uVmzNuDK4QWej"}]')
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.list_updates(url=full_url, **parameters)
-            assert normalize_result(get_updates_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_updates(**parameters)
 
     for parameters in parameter_list:
@@ -6903,14 +6997,15 @@
                 resp = await client.list_updates(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_updates(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_updates(**parameters)
 
     for parameters in parameter_list:
@@ -6926,14 +7021,15 @@
                 resp = await client.list_updates(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_updates(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_updates(**parameters)
 
     for parameters in parameter_list:
@@ -6949,14 +7045,15 @@
                 resp = await client.list_updates(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_updates(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_updates(**parameters)
 
     for parameters in parameter_list:
@@ -6972,14 +7069,15 @@
                 resp = await client.list_updates(url=url_variant, **parameters)
 
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_updates(url=full_url, **parameters)
+
     for parameters in parameter_list:
         aioresponses.get(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.list_updates(**parameters)
 
     for parameters in parameter_list:
@@ -7003,45 +7101,46 @@
 
 @pytest.mark.asyncio
 async def test_create_update(aioresponses: aioresponses):
     url = r'/updates'
     url_variant = r'updates'
     full_url = BASE_URL+r'/updates'
 
-    request_dict = json.loads(r'{"device_id":"enim incididunt in ipsum quis","latest_version":"magna velit aliquip cillum","latest_version_link":"http://MbDqRBByEQRnrHexTQexr.mmMcwHTtG5LNpgZN8S25xYB1GbMREwkXLgPol2Mce"}')
-    request = post_updates_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"device_id":"culpa esse dolore","latest_version":"minim magna","latest_version_link":"https://IncbR.bfnzF7cIrhjd,1W9EMaAzC-1GmY65i,reRg+EUT-LzYBJyYRGXPSJ4O42lEVIqKOr"}')
 
     parameter_list = [{}, ]
+
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"device_id":"enim incididunt in ipsum quis","latest_version":"magna velit aliquip cillum","latest_version_link":"http://MbDqRBByEQRnrHexTQexr.mmMcwHTtG5LNpgZN8S25xYB1GbMREwkXLgPol2Mce"}')
+        response_201_dict = json.loads(r'{"device_id":"culpa esse dolore","latest_version":"minim magna","latest_version_link":"https://IncbR.bfnzF7cIrhjd,1W9EMaAzC-1GmY65i,reRg+EUT-LzYBJyYRGXPSJ4O42lEVIqKOr"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_update(body=request, **parameters)
-            assert normalize_result(post_updates_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"device_id":"enim incididunt in ipsum quis","latest_version":"magna velit aliquip cillum","latest_version_link":"http://MbDqRBByEQRnrHexTQexr.mmMcwHTtG5LNpgZN8S25xYB1GbMREwkXLgPol2Mce"}')
+        response_201_dict = json.loads(r'{"device_id":"culpa esse dolore","latest_version":"minim magna","latest_version_link":"https://IncbR.bfnzF7cIrhjd,1W9EMaAzC-1GmY65i,reRg+EUT-LzYBJyYRGXPSJ4O42lEVIqKOr"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_update(url=url, body=request, **parameters)
-            assert normalize_result(post_updates_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"device_id":"enim incididunt in ipsum quis","latest_version":"magna velit aliquip cillum","latest_version_link":"http://MbDqRBByEQRnrHexTQexr.mmMcwHTtG5LNpgZN8S25xYB1GbMREwkXLgPol2Mce"}')
+        response_201_dict = json.loads(r'{"device_id":"culpa esse dolore","latest_version":"minim magna","latest_version_link":"https://IncbR.bfnzF7cIrhjd,1W9EMaAzC-1GmY65i,reRg+EUT-LzYBJyYRGXPSJ4O42lEVIqKOr"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_update(url=url_variant, body=request, **parameters)
-            assert normalize_result(post_updates_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
 
     for parameters in parameter_list:
-        response_201_dict = json.loads(r'{"device_id":"enim incididunt in ipsum quis","latest_version":"magna velit aliquip cillum","latest_version_link":"http://MbDqRBByEQRnrHexTQexr.mmMcwHTtG5LNpgZN8S25xYB1GbMREwkXLgPol2Mce"}')
+        response_201_dict = json.loads(r'{"device_id":"culpa esse dolore","latest_version":"minim magna","latest_version_link":"https://IncbR.bfnzF7cIrhjd,1W9EMaAzC-1GmY65i,reRg+EUT-LzYBJyYRGXPSJ4O42lEVIqKOr"}')
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=201, payload=response_201_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.create_update(url=full_url, body=request, **parameters)
-            assert normalize_result(post_updates_response_body201_read_to_dict(resp)) == normalize_result(response_201_dict)
+            assert normalize_result(resp) == normalize_result(response_201_dict)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_update(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -7057,14 +7156,15 @@
                 resp = await client.create_update(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_update(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_update(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -7080,14 +7180,15 @@
                 resp = await client.create_update(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=401)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_update(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_update(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -7103,14 +7204,15 @@
                 resp = await client.create_update(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=403)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_update(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_update(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -7126,14 +7228,15 @@
                 resp = await client.create_update(url=url_variant, body=request, **parameters)
 
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=404)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_update(url=full_url, body=request, **parameters)
+
     for parameters in parameter_list:
         aioresponses.post(re.compile(re.escape(full_url)+r'(\?.*)?'), status=500)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.create_update(body=request, **parameters)
 
     for parameters in parameter_list:
@@ -7286,39 +7389,38 @@
 
 @pytest.mark.asyncio
 async def test_patch_update(aioresponses: aioresponses):
     url = r'/updates/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     url_variant = r'updates/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
     full_url = BASE_URL+r'/updates/c799cc2e-cdc5-4143-973a-6f56a5afa82c'
 
-    request_dict = json.loads(r'{"device_id":"enim incididunt in ipsum quis","latest_version":"magna velit aliquip cillum","latest_version_link":"http://MbDqRBByEQRnrHexTQexr.mmMcwHTtG5LNpgZN8S25xYB1GbMREwkXLgPol2Mce"}')
-    request = patch_update_request_body_write_from_dict(request_dict)
+    request = json.loads(r'{"device_id":"culpa esse dolore","latest_version":"minim magna","latest_version_link":"https://IncbR.bfnzF7cIrhjd,1W9EMaAzC-1GmY65i,reRg+EUT-LzYBJyYRGXPSJ4O42lEVIqKOr"}')
 
     parameter_list = [{}, ]
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"device_id":"enim incididunt in ipsum quis","latest_version":"magna velit aliquip cillum","latest_version_link":"http://MbDqRBByEQRnrHexTQexr.mmMcwHTtG5LNpgZN8S25xYB1GbMREwkXLgPol2Mce"}')
+        response_200_dict = json.loads(r'{"device_id":"culpa esse dolore","latest_version":"minim magna","latest_version_link":"https://IncbR.bfnzF7cIrhjd,1W9EMaAzC-1GmY65i,reRg+EUT-LzYBJyYRGXPSJ4O42lEVIqKOr"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.patch_update(url=url, body=request, **parameters)
-            assert normalize_result(patch_update_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"device_id":"enim incididunt in ipsum quis","latest_version":"magna velit aliquip cillum","latest_version_link":"http://MbDqRBByEQRnrHexTQexr.mmMcwHTtG5LNpgZN8S25xYB1GbMREwkXLgPol2Mce"}')
+        response_200_dict = json.loads(r'{"device_id":"culpa esse dolore","latest_version":"minim magna","latest_version_link":"https://IncbR.bfnzF7cIrhjd,1W9EMaAzC-1GmY65i,reRg+EUT-LzYBJyYRGXPSJ4O42lEVIqKOr"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.patch_update(url=url_variant, body=request, **parameters)
-            assert normalize_result(patch_update_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
-        response_200_dict = json.loads(r'{"device_id":"enim incididunt in ipsum quis","latest_version":"magna velit aliquip cillum","latest_version_link":"http://MbDqRBByEQRnrHexTQexr.mmMcwHTtG5LNpgZN8S25xYB1GbMREwkXLgPol2Mce"}')
+        response_200_dict = json.loads(r'{"device_id":"culpa esse dolore","latest_version":"minim magna","latest_version_link":"https://IncbR.bfnzF7cIrhjd,1W9EMaAzC-1GmY65i,reRg+EUT-LzYBJyYRGXPSJ4O42lEVIqKOr"}')
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=200, payload=response_200_dict)
         async with APIClient(BASE_URL) as client:
             resp = await client.patch_update(url=full_url, body=request, **parameters)
-            assert normalize_result(patch_update_response_body200_read_to_dict(resp)) == normalize_result(response_200_dict)
+            assert normalize_result(resp) == normalize_result(response_200_dict)
 
     for parameters in parameter_list:
         aioresponses.patch(re.compile(re.escape(full_url)+r'(\?.*)?'), status=400)
         async with APIClient(BASE_URL) as client:
             with pytest.raises(Exception):
                 resp = await client.patch_update(url=url, body=request, **parameters)
```


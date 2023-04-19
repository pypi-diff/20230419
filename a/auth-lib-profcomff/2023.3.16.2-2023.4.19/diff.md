# Comparing `tmp/auth_lib_profcomff-2023.3.16.2.tar.gz` & `tmp/auth_lib_profcomff-2023.4.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_lib_profcomff-2023.3.16.2.tar", last modified: Thu Mar 16 11:30:19 2023, max compression
+gzip compressed data, was "auth_lib_profcomff-2023.4.19.tar", last modified: Wed Apr 19 12:02:16 2023, max compression
```

## Comparing `auth_lib_profcomff-2023.3.16.2.tar` & `auth_lib_profcomff-2023.4.19.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:30:19.213275 auth_lib_profcomff-2023.3.16.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-03-16 11:30:03.000000 auth_lib_profcomff-2023.3.16.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-16 11:30:19.213275 auth_lib_profcomff-2023.3.16.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-16 11:30:03.000000 auth_lib_profcomff-2023.3.16.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:30:19.213275 auth_lib_profcomff-2023.3.16.2/auth_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 11:30:03.000000 auth_lib_profcomff-2023.3.16.2/auth_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-03-16 11:30:03.000000 auth_lib_profcomff-2023.3.16.2/auth_lib/aiomethods.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-16 11:30:03.000000 auth_lib_profcomff-2023.3.16.2/auth_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-03-16 11:30:03.000000 auth_lib_profcomff-2023.3.16.2/auth_lib/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-03-16 11:30:03.000000 auth_lib_profcomff-2023.3.16.2/auth_lib/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 11:30:19.213275 auth_lib_profcomff-2023.3.16.2/auth_lib_profcomff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-16 11:30:19.000000 auth_lib_profcomff-2023.3.16.2/auth_lib_profcomff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-16 11:30:19.000000 auth_lib_profcomff-2023.3.16.2/auth_lib_profcomff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 11:30:19.000000 auth_lib_profcomff-2023.3.16.2/auth_lib_profcomff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-16 11:30:19.000000 auth_lib_profcomff-2023.3.16.2/auth_lib_profcomff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-16 11:30:19.000000 auth_lib_profcomff-2023.3.16.2/auth_lib_profcomff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 11:30:19.213275 auth_lib_profcomff-2023.3.16.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-16 11:30:03.000000 auth_lib_profcomff-2023.3.16.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:02:16.908690 auth_lib_profcomff-2023.4.19/
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-19 12:02:16.908690 auth_lib_profcomff-2023.4.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:02:16.908690 auth_lib_profcomff-2023.4.19/auth_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/aiomethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:02:16.908690 auth_lib_profcomff-2023.4.19/auth_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/auth_lib/testing/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:02:16.908690 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-04-19 12:02:16.000000 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-19 12:02:16.000000 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:02:16.000000 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-19 12:02:16.000000 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-19 12:02:16.000000 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 12:02:16.000000 auth_lib_profcomff-2023.4.19/auth_lib_profcomff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 12:02:16.908690 auth_lib_profcomff-2023.4.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-19 12:02:02.000000 auth_lib_profcomff-2023.4.19/setup.py
```

### Comparing `auth_lib_profcomff-2023.3.16.2/LICENSE` & `auth_lib_profcomff-2023.4.19/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.3.16.2/auth_lib/aiomethods.py` & `auth_lib_profcomff-2023.4.19/auth_lib/aiomethods.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from typing import Any
 
 import aiohttp
 
-from .exceptions import SessionExpired, AuthFailed, IncorrectData, NotFound
+from .exceptions import AuthFailed, IncorrectData, NotFound, SessionExpired
 
 # See docs on https://api.test.profcomff.com/?urls.primaryName=auth
 
+
 class AsyncAuthLib:
     url: str
 
     def __init__(self, url: str):
         self.url = url
 
     async def email_login(self, email: str, password: str) -> dict[str, Any]:
@@ -24,15 +25,22 @@
 
     async def check_token(self, token: str) -> dict[str, Any]:
         headers = {"Authorization": token}
         async with aiohttp.ClientSession() as session:
             response = await session.get(
                 url=f"{self.url}/me",
                 headers=headers,
-                params={"info": ["groups", "indirect_groups", "session_scopes", "user_scopes"]},
+                params={
+                    "info": [
+                        "groups",
+                        "indirect_groups",
+                        "session_scopes",
+                        "user_scopes",
+                    ]
+                },
             )
         match response.status:
             case 200:
                 return await response.json()
             case 400:
                 raise IncorrectData(response=await response.json())
             case 404:
```

### Comparing `auth_lib_profcomff-2023.3.16.2/auth_lib/exceptions.py` & `auth_lib_profcomff-2023.4.19/auth_lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.3.16.2/auth_lib/fastapi.py` & `auth_lib_profcomff-2023.4.19/auth_lib/fastapi.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from urllib.parse import urljoin
 from warnings import warn
 
 import aiohttp
 from fastapi.exceptions import HTTPException
 from fastapi.openapi.models import APIKey, APIKeyIn
 from fastapi.security.base import SecurityBase
+from pydantic import BaseSettings
 from starlette.requests import Request
 from starlette.status import HTTP_403_FORBIDDEN
-from pydantic import BaseSettings
 
 
 class UnionAuthSettings(BaseSettings):
     AUTH_URL: str = "https://api.test.profcomff.com/auth/"
     AUTH_AUTO_ERROR: bool = True
     AUTH_ALLOW_NONE: bool = False
 
@@ -28,24 +28,31 @@
     settings = UnionAuthSettings()
 
     def __init__(
         self,
         scopes: list[str] = [],
         auto_error: bool | None = None,
         allow_none: bool | None = None,
-        auth_url = None,  # Для обратной совместимости
+        auth_url=None,  # Для обратной совместимости
     ) -> None:
         if auth_url is not None:
-            warn("auth_url in args deprecated, use AUTH_URL env instead", DeprecationWarning)
+            warn(
+                "auth_url in args deprecated, use AUTH_URL env instead",
+                DeprecationWarning,
+            )
         super().__init__()
         self.auth_url = auth_url or self.settings.AUTH_URL
-        if not self.auth_url.endswith('/'):
-            self.auth_url = self.auth_url + '/'
-        self.auto_error = auto_error if auto_error is not None else self.settings.AUTH_AUTO_ERROR
-        self.allow_none = allow_none if allow_none is not None else self.settings.AUTH_ALLOW_NONE
+        if not self.auth_url.endswith("/"):
+            self.auth_url = self.auth_url + "/"
+        self.auto_error = (
+            auto_error if auto_error is not None else self.settings.AUTH_AUTO_ERROR
+        )
+        self.allow_none = (
+            allow_none if allow_none is not None else self.settings.AUTH_ALLOW_NONE
+        )
         self.scopes = scopes
 
     def _except(self):
         if self.auto_error:
             raise HTTPException(
                 status_code=HTTP_403_FORBIDDEN, detail="Not authenticated"
             )
@@ -61,18 +68,22 @@
             return None
         if not token:
             return self._except()
         async with aiohttp.request(
             "GET",
             urljoin(self.auth_url, "me"),
             headers={"Authorization": token},
-            params={"info": ["groups", "indirect_groups", "session_scopes", "user_scopes"]},
+            params={
+                "info": ["groups", "indirect_groups", "session_scopes", "user_scopes"]
+            },
         ) as r:
             status_code = r.status
             user_session = await r.json()
         if status_code != 200:
             self._except()
-        session_scopes = set([scope["name"].lower() for scope in user_session["session_scopes"]])
+        session_scopes = set(
+            [scope["name"].lower() for scope in user_session["session_scopes"]]
+        )
         required_scopes = set([scope.lower() for scope in self.scopes])
         if required_scopes - session_scopes:
             self._except()
         return user_session
```

### Comparing `auth_lib_profcomff-2023.3.16.2/auth_lib/methods.py` & `auth_lib_profcomff-2023.4.19/auth_lib/methods.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Any
 
 import requests
 
-from .exceptions import SessionExpired, AuthFailed, IncorrectData, NotFound
-
+from .exceptions import AuthFailed, IncorrectData, NotFound, SessionExpired
 
 # See docs on https://api.test.profcomff.com/?urls.primaryName=auth
 
 
 class AuthLib:
     url: str
 
@@ -24,15 +23,17 @@
                 raise AuthFailed(response=response.json()["body"])
 
     def check_token(self, token: str) -> dict[str, Any]:
         headers = {"Authorization": token}
         response = requests.get(
             url=f"{self.url}/me",
             headers=headers,
-            params={"info": ["groups", "indirect_groups", "session_scopes", "user_scopes"]},
+            params={
+                "info": ["groups", "indirect_groups", "session_scopes", "user_scopes"]
+            },
         )
         match response.status_code:
             case 200:
                 return response.json()
             case 400:
                 raise IncorrectData(response=response.json()["body"])
             case 404:
```

### Comparing `auth_lib_profcomff-2023.3.16.2/setup.py` & `auth_lib_profcomff-2023.4.19/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
 setup(
     name="auth_lib_profcomff",
-    version="2023.03.16.2",
+    version="2023.04.19",
     author="Semyon Grigoriev",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/profcomff/auth-lib",
     packages=find_packages(),
     install_requires=["requests", "aiohttp", "setuptools"],
     extras_require={
         "fastapi": ["fastapi", "starlette", "pydantic"],
+        "testing": ["pytest"],
     },
+    entry_points={"pytest11": ["pytest_auth_lib = auth_lib.testing"]},
     classifiers=[
         "Programming Language :: Python :: 3.11",
     ],
 )
```


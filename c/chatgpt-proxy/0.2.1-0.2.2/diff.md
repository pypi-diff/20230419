# Comparing `tmp/chatgpt-proxy-0.2.1.tar.gz` & `tmp/chatgpt-proxy-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-proxy-0.2.1.tar", last modified: Tue Apr 18 14:52:54 2023, max compression
+gzip compressed data, was "chatgpt-proxy-0.2.2.tar", last modified: Wed Apr 19 13:52:45 2023, max compression
```

## Comparing `chatgpt-proxy-0.2.1.tar` & `chatgpt-proxy-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:52:54.848481 chatgpt-proxy-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-18 14:52:43.000000 chatgpt-proxy-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-18 14:52:54.848481 chatgpt-proxy-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-18 14:52:43.000000 chatgpt-proxy-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:52:54.844480 chatgpt-proxy-0.2.1/chatgpt_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 14:52:43.000000 chatgpt-proxy-0.2.1/chatgpt_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-18 14:52:43.000000 chatgpt-proxy-0.2.1/chatgpt_proxy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-04-18 14:52:43.000000 chatgpt-proxy-0.2.1/chatgpt_proxy/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:52:54.848481 chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-18 14:52:54.000000 chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-18 14:52:54.000000 chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:52:54.000000 chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 14:52:54.000000 chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 14:52:54.000000 chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-18 14:52:43.000000 chatgpt-proxy-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 14:52:54.848481 chatgpt-proxy-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:52:45.968959 chatgpt-proxy-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-19 13:52:35.000000 chatgpt-proxy-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-19 13:52:45.968959 chatgpt-proxy-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-19 13:52:35.000000 chatgpt-proxy-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:52:45.968959 chatgpt-proxy-0.2.2/chatgpt_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 13:52:35.000000 chatgpt-proxy-0.2.2/chatgpt_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-19 13:52:35.000000 chatgpt-proxy-0.2.2/chatgpt_proxy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-19 13:52:35.000000 chatgpt-proxy-0.2.2/chatgpt_proxy/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:52:45.968959 chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-19 13:52:45.000000 chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-19 13:52:45.000000 chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:52:45.000000 chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 13:52:45.000000 chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 13:52:45.000000 chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-19 13:52:35.000000 chatgpt-proxy-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:52:45.968959 chatgpt-proxy-0.2.2/setup.cfg
```

### Comparing `chatgpt-proxy-0.2.1/LICENSE` & `chatgpt-proxy-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-proxy-0.2.1/PKG-INFO` & `chatgpt-proxy-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-proxy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Reverse proxy for OpenAI chatgpt website API
 Author: 18870
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `chatgpt-proxy-0.2.1/README.md` & `chatgpt-proxy-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `chatgpt-proxy-0.2.1/chatgpt_proxy/__main__.py` & `chatgpt-proxy-0.2.2/chatgpt_proxy/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import asyncio
 import logging
 from contextlib import asynccontextmanager
 
 import uvicorn
 from fastapi import FastAPI, Header
 from pydantic import BaseModel, BaseSettings, Field
 
@@ -38,36 +37,55 @@
         user_agent=env.user_agent,
         access_token=env.access_token,
         trust=env.trust,
     )
 
     @asynccontextmanager
     async def lifespan(app: FastAPI):
-        refresh_puid_task = asyncio.create_task(proxy._refresh_task())
+        await proxy.check_cf()
         yield
 
     app = FastAPI(lifespan=lifespan)
     proxy.attach(app, path="/backend-api")
 
     if env.mod_access_token:
-        logger.info("Mod access token found, enable /moderation/update_info endpoint")
+        logger.info("Mod access token found, enable /moderation/* endpoint")
 
         class Info(BaseModel):
             cf_clearance: str = None
             access_token: str = None
+            user_agent: str = None
 
         @app.post("/moderation/update_info", status_code=200)
-        async def update_info(info: Info, authorization: str = Header(...)):
-            if authorization == env.mod_access_token:
-                if info.access_token:
-                    logger.info("New access token found")
-                    proxy.access_token = info.access_token
-                if info.cf_clearance:
-                    logger.info(f"New cf_clearance: {info.cf_clearance}")
-                    proxy.cf_clearance = info.cf_clearance
-            if await proxy._refresh_puid():
-                logger.info("New info is validated")
+        async def update_info(
+            info: Info,
+            authorization: str = Header(...),
+            user_agent: str = Header(...),
+        ):
+            if authorization != env.mod_access_token:
+                logger.error("Invalid authorization")
+                return {"message": "invalid authorization"}
+
+            if info.access_token:
+                logger.info("New access token found")
+                proxy.access_token = info.access_token
+            if info.cf_clearance:
+                logger.info(f"New cf_clearance: {info.cf_clearance}")
+                proxy.cf_clearance = info.cf_clearance
+            proxy.user_agent = info.user_agent or user_agent
+
+            if await proxy.check_cf():
+                logger.info("New info is valid")
+                return {"message": "ok"}
             else:
                 logger.error("Failed to validate new info")
-            return {"status": "ok"}
+                return {"message": "failed"}
+
+        @app.get("/moderation/status", status_code=200)
+        async def status(authorization: str = Header(...)):
+            if authorization != env.mod_access_token:
+                logger.error("Invalid authorization")
+                return {"message": "invalid authorization"}
+
+            return {"message": "ok", "status": proxy.valid_state}
 
     uvicorn.run(app, host=env.host, port=env.port)
```

### Comparing `chatgpt-proxy-0.2.1/chatgpt_proxy/proxy.py` & `chatgpt-proxy-0.2.2/chatgpt_proxy/proxy.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,56 +23,65 @@
         "TRACE",
         "CONNECT",
     ]
 
     def __init__(self, base_url: str) -> None:
         self.base_url = base_url
         self.client = httpx.AsyncClient(base_url=base_url)
+
         _url = urlparse(base_url)
         self._domain = _url.netloc
         self._origin = urlunparse(
             ParseResult(
                 scheme=_url.scheme,
                 netloc=_url.netloc,
                 path="",
                 params="",
                 query="",
                 fragment="",
             )
         )
+        self._preset_headers = {
+            "host": self._domain,
+            "origin": self._origin,
+            "referer": self.base_url,
+        }
 
     async def _prepare_cookies(self, request: Request):
         return request.cookies.copy()
 
     async def _prepare_headers(self, request: Request):
         # Note that all header keys are lowercased
         headers = dict(request.headers)
 
         # cookie in headers have higher priority
         # so remove it here and let cookies parameter take effect
         headers.pop("cookie", None)
 
         # preset header
-        headers["host"] = self._domain
-        headers["origin"] = self._origin
-        headers["referer"] = self.base_url
+        headers.update(self._preset_headers)
         return headers
 
+    async def _process_response(self, response: httpx.Response):
+        pass
+
     async def proxy(self, request: Request, path: str):
         # https://github.com/tiangolo/fastapi/discussions/7382#discussioncomment-5136454
         logger.info(f"Proxying {request.method} {request.url}")
         rp_resp = await self._send_request(
             path=path,
             query=request.url.query.encode("utf-8"),
             method=request.method,
             headers=await self._prepare_headers(request),
             cookies=await self._prepare_cookies(request),
             content=request.stream(),
         )
 
+        await self._process_response(rp_resp)
+
         # Handle Set-Cookie headers
         headers = rp_resp.headers.copy()
         headers.pop("set-cookie", None)
 
         resp = StreamingResponse(
             rp_resp.aiter_raw(),
             status_code=rp_resp.status_code,
@@ -98,52 +107,63 @@
             description=f"Reverse proxy of {self.base_url}",
             **kwargs,
         )
 
 
 class WebChatGPTProxy(ReverseProxy):
     def __init__(
-        self, cf_clearance: str, user_agent: str, access_token: Optional[str] = None, trust: bool = False
+        self,
+        cf_clearance: str,
+        user_agent: str,
+        access_token: Optional[str] = None,
+        trust: bool = False,
     ) -> None:
         """
         :param puid: from `_puid` cookie
         :param access_token: from openai `access_token`
                              obtained from here https://chat.openai.com/api/auth/session
                              Used to refresh puid
         :param trust: Trust requests from any client.
                       When set to True, any requests without an access_token will be given the above access_token.
                       Default to False, which will only use for refresh puid.
         """
         super().__init__(base_url="https://chat.openai.com/backend-api/")
         self.cf_clearance = cf_clearance
-        self.ua = user_agent
+        self.user_agent = user_agent
         self.access_token = access_token
         self.trust = trust
         self._app: Optional[FastAPI] = None
         self._path: Optional[str] = None
+        self.valid_state = False
 
     async def _prepare_cookies(self, request: Request):
         cookies = await super()._prepare_cookies(request)
         cookies.setdefault("cf_clearance", self.cf_clearance)
         return cookies
 
     async def _prepare_headers(self, request: Request):
         headers = await super()._prepare_headers(request)
-        headers["origin"] = "https://chat.openai.com"
         headers["referer"] = "https://chat.openai.com"
-        headers["user-agent"] = self.ua
+        headers["user-agent"] = self.user_agent
         if self.trust and self.access_token:
             headers.setdefault("authorization", f"Bearer {self.access_token}")
         return headers
 
+    async def _process_response(self, response: httpx.Response):
+        if response.status_code == 200:
+            self.valid_state = True
+        elif response.status_code == 403:
+            logger.error("403 Forbidden found")
+            self.valid_state = False
+
     async def _refresh_puid(self) -> bool:
         """
         Send requests to /models through reverse proxy (current FastAPI app) to get a new puid
-        
-        Use to see if you pass cloudflare
+
+        Deprecated
         """
         if self._app is None:
             logger.info("Not attached to any FastAPI app, skip")
         async with httpx.AsyncClient(
             app=self._app, base_url=f"https://chat.openai.com{self._path}"
         ) as client:
             resp = await client.get(
@@ -157,23 +177,42 @@
             else:
                 logger.error("Failed to get puid")
                 logger.error(f"Cookies: {resp.cookies}")
                 logger.error(f"Response: \n{resp.text}")
                 return False
 
     async def _refresh_task(self) -> None:
+        """
+        Deprecated
+        """
         if self.access_token is None:
             logger.info("access_token not found, skip")
             return
 
         try:
             await self._refresh_puid()
         except Exception as e:
             logger.exception(e)
             # await asyncio.sleep(60 * 60)
             # continue
         # await asyncio.sleep(60 * 60 * 6)
 
+    async def check_cf(self) -> bool:
+        if self._app is None:
+            logger.info("Not attached to any FastAPI app, cannot perform check")
+        async with httpx.AsyncClient(
+            app=self._app, base_url=f"https://chat.openai.com{self._path}"
+        ) as client:
+            resp = await client.get("/models")
+            if resp.status_code in (200, 401):
+                logger.info(f"Check passed, status code: {resp.status_code}")
+                self.valid_state = True
+                return True
+            elif resp.status_code == 403:
+                logger.error(f"Check failed, status code 403")
+                logger.error(f"Response: \n{resp.text}")
+                return False
+
     def attach(self, app: FastAPI, path: str) -> None:
         super().attach(app=app, path=path, include_in_schema=self.trust)
         self._app = app
         self._path = path
```

### Comparing `chatgpt-proxy-0.2.1/chatgpt_proxy.egg-info/PKG-INFO` & `chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-proxy
-Version: 0.2.1
+Version: 0.2.2
 Summary: Reverse proxy for OpenAI chatgpt website API
 Author: 18870
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


# Comparing `tmp/chatgpt-proxy-0.2.2.tar.gz` & `tmp/chatgpt-proxy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-proxy-0.2.2.tar", last modified: Wed Apr 19 13:52:45 2023, max compression
+gzip compressed data, was "chatgpt-proxy-0.2.3.tar", last modified: Wed Apr 19 16:33:13 2023, max compression
```

## Comparing `chatgpt-proxy-0.2.2.tar` & `chatgpt-proxy-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:52:45.968959 chatgpt-proxy-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-19 13:52:35.000000 chatgpt-proxy-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-19 13:52:45.968959 chatgpt-proxy-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-04-19 13:52:35.000000 chatgpt-proxy-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:52:45.968959 chatgpt-proxy-0.2.2/chatgpt_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 13:52:35.000000 chatgpt-proxy-0.2.2/chatgpt_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-19 13:52:35.000000 chatgpt-proxy-0.2.2/chatgpt_proxy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-04-19 13:52:35.000000 chatgpt-proxy-0.2.2/chatgpt_proxy/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:52:45.968959 chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-19 13:52:45.000000 chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-19 13:52:45.000000 chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:52:45.000000 chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 13:52:45.000000 chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 13:52:45.000000 chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-19 13:52:35.000000 chatgpt-proxy-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 13:52:45.968959 chatgpt-proxy-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:33:13.687107 chatgpt-proxy-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34881 2023-04-19 16:33:02.000000 chatgpt-proxy-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-19 16:33:13.687107 chatgpt-proxy-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-04-19 16:33:02.000000 chatgpt-proxy-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:33:13.683107 chatgpt-proxy-0.2.3/chatgpt_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 16:33:02.000000 chatgpt-proxy-0.2.3/chatgpt_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-04-19 16:33:02.000000 chatgpt-proxy-0.2.3/chatgpt_proxy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-04-19 16:33:02.000000 chatgpt-proxy-0.2.3/chatgpt_proxy/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:33:13.687107 chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-04-19 16:33:13.000000 chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-19 16:33:13.000000 chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:33:13.000000 chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 16:33:13.000000 chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 16:33:13.000000 chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-19 16:33:02.000000 chatgpt-proxy-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:33:13.687107 chatgpt-proxy-0.2.3/setup.cfg
```

### Comparing `chatgpt-proxy-0.2.2/LICENSE` & `chatgpt-proxy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-proxy-0.2.2/PKG-INFO` & `chatgpt-proxy-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-proxy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Reverse proxy for OpenAI chatgpt website API
 Author: 18870
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -23,30 +23,33 @@
 
 ## Usage
 
 For how to get a usable `cf_clearance` cookie, checkout issue [#1](https://github.com/18870/chatgpt-proxy/issues/1) (Chinese only sorry)
 
 ### Run as a service
 Set these environment variables:
-- `CF_CLEARANCE`: Cookie `cf_clearance`
-- `USER_AGENT`: User-agent of your browser when you get the cookie `cf_clearance`
+- `CF_CLEARANCE`: (Optional) Cookie `cf_clearance`
+- `USER_AGENT`: (Optional) User-agent of your browser when you get the cookie `cf_clearance`
 - `ACCESS_TOKEN`: (Optional) Obtains from [here](https://chat.openai.com/api/auth/session)
+- `PUID`: (Optional) Cookie `_puid`, still needed to start a conversation for plus account (?)
+    When set a plus account's access_token, this can be automatically refresh
 - `PROXY_TRUST_CLIENT`: (Optional) Trust requests from any client.  
     When set to `True`, any requests without an access_token will be given the above access_token.  
     Default to `False`, which will only use for refresh puid.
 - `HOST`: (Optional) Listen on host, default to `127.0.0.1`
 - `PORT`: (Optional) Listen on port, default to `7800`
 - `MOD_ACCESS_TOKEN`: (Optional) Update info like cf_clearance through http request 
     requires you set this access_token in `Authorization` Header 
 
 Or create a `.env` file with your environment variables at where you want to run the proxy:
 ```ini
 cf_clearance=YOUR_CF_CLEARANCE
 user_agent=YOUR_USER_AGENT
 access_token=YOUR_ACCESS_TOKEN
+puid=ANY_VALID_PUID
 proxy_trust_client=False
 host=127.0.0.1
 port=7800
 mod_access_token=YOUR_MOD_ACCESS_TOKEN
 ```
 
 Note that environment variables will override the values in `.env` file.
@@ -69,14 +72,15 @@
 proxy.attach(app, path="/backend-api")
 ```
 
 class `WebChatGPTProxy`:
 - `cf_clearance`: Cookie `cf_clearance`
 - `user_agent`: User-agent of your browser when you get the cookie `cf_clearance`
 - `access_token`: (Optional)
+- `puid`: (Optional)
 - `trust`: (Optional) Trust requests from any client.
     When set to True, any requests without an access_token will be given the above access_token.
     Default to False, which will only use for refresh puid.
 
 ### Behind a http proxy
 **You need to use the same ip address you used to get the cookie `cf_clearance`**
```

### Comparing `chatgpt-proxy-0.2.2/README.md` & `chatgpt-proxy-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,30 +13,33 @@
 
 ## Usage
 
 For how to get a usable `cf_clearance` cookie, checkout issue [#1](https://github.com/18870/chatgpt-proxy/issues/1) (Chinese only sorry)
 
 ### Run as a service
 Set these environment variables:
-- `CF_CLEARANCE`: Cookie `cf_clearance`
-- `USER_AGENT`: User-agent of your browser when you get the cookie `cf_clearance`
+- `CF_CLEARANCE`: (Optional) Cookie `cf_clearance`
+- `USER_AGENT`: (Optional) User-agent of your browser when you get the cookie `cf_clearance`
 - `ACCESS_TOKEN`: (Optional) Obtains from [here](https://chat.openai.com/api/auth/session)
+- `PUID`: (Optional) Cookie `_puid`, still needed to start a conversation for plus account (?)
+    When set a plus account's access_token, this can be automatically refresh
 - `PROXY_TRUST_CLIENT`: (Optional) Trust requests from any client.  
     When set to `True`, any requests without an access_token will be given the above access_token.  
     Default to `False`, which will only use for refresh puid.
 - `HOST`: (Optional) Listen on host, default to `127.0.0.1`
 - `PORT`: (Optional) Listen on port, default to `7800`
 - `MOD_ACCESS_TOKEN`: (Optional) Update info like cf_clearance through http request 
     requires you set this access_token in `Authorization` Header 
 
 Or create a `.env` file with your environment variables at where you want to run the proxy:
 ```ini
 cf_clearance=YOUR_CF_CLEARANCE
 user_agent=YOUR_USER_AGENT
 access_token=YOUR_ACCESS_TOKEN
+puid=ANY_VALID_PUID
 proxy_trust_client=False
 host=127.0.0.1
 port=7800
 mod_access_token=YOUR_MOD_ACCESS_TOKEN
 ```
 
 Note that environment variables will override the values in `.env` file.
@@ -59,14 +62,15 @@
 proxy.attach(app, path="/backend-api")
 ```
 
 class `WebChatGPTProxy`:
 - `cf_clearance`: Cookie `cf_clearance`
 - `user_agent`: User-agent of your browser when you get the cookie `cf_clearance`
 - `access_token`: (Optional)
+- `puid`: (Optional)
 - `trust`: (Optional) Trust requests from any client.
     When set to True, any requests without an access_token will be given the above access_token.
     Default to False, which will only use for refresh puid.
 
 ### Behind a http proxy
 **You need to use the same ip address you used to get the cookie `cf_clearance`**
```

### Comparing `chatgpt-proxy-0.2.2/chatgpt_proxy/__main__.py` & `chatgpt-proxy-0.2.3/chatgpt_proxy/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import logging
 from contextlib import asynccontextmanager
 
 import uvicorn
 from fastapi import FastAPI, Header
 from pydantic import BaseModel, BaseSettings, Field
 
@@ -13,16 +14,16 @@
     handlers=[logging.StreamHandler()],
 )
 
 logger = logging.getLogger(__name__)
 
 
 class Settings(BaseSettings):
-    cf_clearance: str
-    user_agent: str
+    cf_clearance: str = None
+    user_agent: str = None
 
     access_token: str = None
     host: str = "127.0.0.1"
     port: int = 7800
     trust: bool = Field(default=False, env="proxy_trust_client")
     mod_access_token: str = None
 
@@ -37,15 +38,15 @@
         user_agent=env.user_agent,
         access_token=env.access_token,
         trust=env.trust,
     )
 
     @asynccontextmanager
     async def lifespan(app: FastAPI):
-        await proxy.check_cf()
+        asyncio.create_task(proxy._refresh_task())
         yield
 
     app = FastAPI(lifespan=lifespan)
     proxy.attach(app, path="/backend-api")
 
     if env.mod_access_token:
         logger.info("Mod access token found, enable /moderation/* endpoint")
```

### Comparing `chatgpt-proxy-0.2.2/chatgpt_proxy/proxy.py` & `chatgpt-proxy-0.2.3/chatgpt_proxy/proxy.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,37 +111,42 @@
 
 class WebChatGPTProxy(ReverseProxy):
     def __init__(
         self,
         cf_clearance: str,
         user_agent: str,
         access_token: Optional[str] = None,
+        puid: Optional[str] = None,
         trust: bool = False,
     ) -> None:
         """
-        :param puid: from `_puid` cookie
+        :param cf_clearance: from `cf_clearance` cookie
+        :param user_agent: from `user-agent` header
         :param access_token: from openai `access_token`
                              obtained from here https://chat.openai.com/api/auth/session
                              Used to refresh puid
+        :param puid: from `_puid` cookie
         :param trust: Trust requests from any client.
                       When set to True, any requests without an access_token will be given the above access_token.
                       Default to False, which will only use for refresh puid.
         """
         super().__init__(base_url="https://chat.openai.com/backend-api/")
         self.cf_clearance = cf_clearance
         self.user_agent = user_agent
         self.access_token = access_token
+        self.puid = puid
         self.trust = trust
         self._app: Optional[FastAPI] = None
         self._path: Optional[str] = None
         self.valid_state = False
 
     async def _prepare_cookies(self, request: Request):
         cookies = await super()._prepare_cookies(request)
         cookies.setdefault("cf_clearance", self.cf_clearance)
+        cookies.setdefault("_puid", self.puid)
         return cookies
 
     async def _prepare_headers(self, request: Request):
         headers = await super()._prepare_headers(request)
         headers["referer"] = "https://chat.openai.com"
         headers["user-agent"] = self.user_agent
         if self.trust and self.access_token:
@@ -177,38 +182,41 @@
             else:
                 logger.error("Failed to get puid")
                 logger.error(f"Cookies: {resp.cookies}")
                 logger.error(f"Response: \n{resp.text}")
                 return False
 
     async def _refresh_task(self) -> None:
-        """
-        Deprecated
-        """
         if self.access_token is None:
             logger.info("access_token not found, skip")
             return
 
         try:
-            await self._refresh_puid()
+            await self.check_cf()
         except Exception as e:
             logger.exception(e)
             # await asyncio.sleep(60 * 60)
             # continue
         # await asyncio.sleep(60 * 60 * 6)
 
     async def check_cf(self) -> bool:
         if self._app is None:
             logger.info("Not attached to any FastAPI app, cannot perform check")
         async with httpx.AsyncClient(
             app=self._app, base_url=f"https://chat.openai.com{self._path}"
         ) as client:
-            resp = await client.get("/models")
+            resp = await client.get(
+                "/models", headers={"authorization": f"Bearer {self.access_token}"}
+            )
             if resp.status_code in (200, 401):
                 logger.info(f"Check passed, status code: {resp.status_code}")
+                puid = resp.cookies.get("_puid")
+                if puid:
+                    logger.info(f"puid: {puid[:15]}...{puid[30:40]}...")
+                    self.puid = puid
                 self.valid_state = True
                 return True
             elif resp.status_code == 403:
                 logger.error(f"Check failed, status code 403")
                 logger.error(f"Response: \n{resp.text}")
                 return False
```

### Comparing `chatgpt-proxy-0.2.2/chatgpt_proxy.egg-info/PKG-INFO` & `chatgpt-proxy-0.2.3/chatgpt_proxy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-proxy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Reverse proxy for OpenAI chatgpt website API
 Author: 18870
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -23,30 +23,33 @@
 
 ## Usage
 
 For how to get a usable `cf_clearance` cookie, checkout issue [#1](https://github.com/18870/chatgpt-proxy/issues/1) (Chinese only sorry)
 
 ### Run as a service
 Set these environment variables:
-- `CF_CLEARANCE`: Cookie `cf_clearance`
-- `USER_AGENT`: User-agent of your browser when you get the cookie `cf_clearance`
+- `CF_CLEARANCE`: (Optional) Cookie `cf_clearance`
+- `USER_AGENT`: (Optional) User-agent of your browser when you get the cookie `cf_clearance`
 - `ACCESS_TOKEN`: (Optional) Obtains from [here](https://chat.openai.com/api/auth/session)
+- `PUID`: (Optional) Cookie `_puid`, still needed to start a conversation for plus account (?)
+    When set a plus account's access_token, this can be automatically refresh
 - `PROXY_TRUST_CLIENT`: (Optional) Trust requests from any client.  
     When set to `True`, any requests without an access_token will be given the above access_token.  
     Default to `False`, which will only use for refresh puid.
 - `HOST`: (Optional) Listen on host, default to `127.0.0.1`
 - `PORT`: (Optional) Listen on port, default to `7800`
 - `MOD_ACCESS_TOKEN`: (Optional) Update info like cf_clearance through http request 
     requires you set this access_token in `Authorization` Header 
 
 Or create a `.env` file with your environment variables at where you want to run the proxy:
 ```ini
 cf_clearance=YOUR_CF_CLEARANCE
 user_agent=YOUR_USER_AGENT
 access_token=YOUR_ACCESS_TOKEN
+puid=ANY_VALID_PUID
 proxy_trust_client=False
 host=127.0.0.1
 port=7800
 mod_access_token=YOUR_MOD_ACCESS_TOKEN
 ```
 
 Note that environment variables will override the values in `.env` file.
@@ -69,14 +72,15 @@
 proxy.attach(app, path="/backend-api")
 ```
 
 class `WebChatGPTProxy`:
 - `cf_clearance`: Cookie `cf_clearance`
 - `user_agent`: User-agent of your browser when you get the cookie `cf_clearance`
 - `access_token`: (Optional)
+- `puid`: (Optional)
 - `trust`: (Optional) Trust requests from any client.
     When set to True, any requests without an access_token will be given the above access_token.
     Default to False, which will only use for refresh puid.
 
 ### Behind a http proxy
 **You need to use the same ip address you used to get the cookie `cf_clearance`**
```


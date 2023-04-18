# Comparing `tmp/fps_login-0.1.3.tar.gz` & `tmp/fps_login-0.1.4.tar.gz`

## Comparing `fps_login-0.1.3.tar` & `fps_login-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fps_login-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/__init__.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/main.py
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/routes.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/static/index.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/static/favicons/favicon-busy-1.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/static/favicons/favicon-busy-2.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/static/favicons/favicon-busy-3.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/static/favicons/favicon-file.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/static/favicons/favicon-notebook.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/static/favicons/favicon-terminal.ico
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/static/favicons/favicon.ico
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/static/logo/github.svg
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/static/logo/logo.png
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 fps_login-0.1.3/fps_login/static/style/index.css
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_login-0.1.3/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_login-0.1.3/COPYING.md
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 fps_login-0.1.3/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 fps_login-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 fps_login-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 fps_login-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/__init__.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/main.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/routes.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/static/index.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/static/favicons/favicon-busy-1.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/static/favicons/favicon-busy-2.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/static/favicons/favicon-busy-3.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/static/favicons/favicon-file.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/static/favicons/favicon-notebook.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/static/favicons/favicon-terminal.ico
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/static/favicons/favicon.ico
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/static/logo/github.svg
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/static/logo/logo.png
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 fps_login-0.1.4/fps_login/static/style/index.css
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_login-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_login-0.1.4/COPYING.md
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 fps_login-0.1.4/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 fps_login-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 fps_login-0.1.4/PKG-INFO
```

### Comparing `fps_login-0.1.3/fps_login/routes.py` & `fps_login-0.1.4/fps_login/routes.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from pathlib import Path
 from typing import Optional, cast
 
-from fastapi import APIRouter
 from fastapi.responses import FileResponse
 from fastapi.staticfiles import StaticFiles
 from jupyverse_api.app import App
 from jupyverse_api.auth import AuthConfig
 from jupyverse_api.login import Login
 
 
@@ -17,25 +16,21 @@
     def __init__(
         self,
         app: App,
         auth_config: AuthConfig,
     ) -> None:
         super().__init__(app)
 
-        router = APIRouter()
-        prefix_static = Path(__file__).parent / "static"
+        self.prefix_static = Path(__file__).parent / "static"
 
         # fps_login needs an AuthConfig that has a login_url, such as fps_auth's config
         auth_config = cast(_AuthConfig, auth_config)
         auth_config.login_url = "/login"
 
         self.mount(
             "/static/login",
-            StaticFiles(directory=prefix_static),
+            StaticFiles(directory=self.prefix_static),
             name="static",
         )
 
-        @router.get("/login")
-        async def api_login():
-            return FileResponse(prefix_static / "index.html")
-
-        self.include_router(router)
+    async def get_login(self):
+        return FileResponse(self.prefix_static / "index.html")
```

### Comparing `fps_login-0.1.3/fps_login/static/index.html` & `fps_login-0.1.4/fps_login/static/index.html`

 * *Files identical despite different names*

### Comparing `fps_login-0.1.3/fps_login/static/favicons/favicon-busy-1.ico` & `fps_login-0.1.4/fps_login/static/favicons/favicon-busy-1.ico`

 * *Files identical despite different names*

### Comparing `fps_login-0.1.3/fps_login/static/favicons/favicon-busy-2.ico` & `fps_login-0.1.4/fps_login/static/favicons/favicon-busy-2.ico`

 * *Files identical despite different names*

### Comparing `fps_login-0.1.3/fps_login/static/favicons/favicon-busy-3.ico` & `fps_login-0.1.4/fps_login/static/favicons/favicon-busy-3.ico`

 * *Files identical despite different names*

### Comparing `fps_login-0.1.3/fps_login/static/favicons/favicon-file.ico` & `fps_login-0.1.4/fps_login/static/favicons/favicon-file.ico`

 * *Files identical despite different names*

### Comparing `fps_login-0.1.3/fps_login/static/favicons/favicon-notebook.ico` & `fps_login-0.1.4/fps_login/static/favicons/favicon-notebook.ico`

 * *Files identical despite different names*

### Comparing `fps_login-0.1.3/fps_login/static/favicons/favicon-terminal.ico` & `fps_login-0.1.4/fps_login/static/favicons/favicon-terminal.ico`

 * *Files identical despite different names*

### Comparing `fps_login-0.1.3/fps_login/static/favicons/favicon.ico` & `fps_login-0.1.4/fps_login/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `fps_login-0.1.3/fps_login/static/logo/github.svg` & `fps_login-0.1.4/fps_login/static/logo/github.svg`

 * *Files identical despite different names*

### Comparing `fps_login-0.1.3/fps_login/static/logo/logo.png` & `fps_login-0.1.4/fps_login/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `fps_login-0.1.3/fps_login/static/style/index.css` & `fps_login-0.1.4/fps_login/static/style/index.css`

 * *Files identical despite different names*

### Comparing `fps_login-0.1.3/.gitignore` & `fps_login-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_login-0.1.3/COPYING.md` & `fps_login-0.1.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_login-0.1.3/pyproject.toml` & `fps_login-0.1.4/pyproject.toml`

 * *Files identical despite different names*


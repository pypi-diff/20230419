# Comparing `tmp/fps_jupyterlab-0.1.3.tar.gz` & `tmp/fps_jupyterlab-0.1.4.tar.gz`

## Comparing `fps_jupyterlab-0.1.3.tar` & `fps_jupyterlab-0.1.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.3/fps_jupyterlab/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.3/fps_jupyterlab/index.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.3/fps_jupyterlab/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.3/fps_jupyterlab/py.typed
--rw-r--r--   0        0        0     6692 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.3/fps_jupyterlab/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.3/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.3/COPYING.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.3/README.md
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.4/fps_jupyterlab/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.4/fps_jupyterlab/index.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.4/fps_jupyterlab/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.4/fps_jupyterlab/py.typed
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.4/fps_jupyterlab/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.4/COPYING.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.4/README.md
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.4/PKG-INFO
```

### Comparing `fps_jupyterlab-0.1.3/fps_jupyterlab/index.py` & `fps_jupyterlab-0.1.4/fps_jupyterlab/index.py`

 * *Files identical despite different names*

### Comparing `fps_jupyterlab-0.1.3/fps_jupyterlab/main.py` & `fps_jupyterlab-0.1.4/fps_jupyterlab/main.py`

 * *Files identical despite different names*

### Comparing `fps_jupyterlab-0.1.3/fps_jupyterlab/routes.py` & `fps_jupyterlab-0.1.4/fps_jupyterlab/routes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from http import HTTPStatus
 from pathlib import Path
 
 import jupyterlab as jupyterlab_module  # type: ignore
-from fastapi import APIRouter, Depends, Response
+from fastapi import Response
 from fastapi.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.frontend import FrontendConfig
 from jupyverse_api.jupyterlab import JupyterLab, JupyterLabConfig
 from jupyverse_api.lab import Lab
@@ -21,93 +21,90 @@
         self,
         app: App,
         jupyterlab_config: JupyterLabConfig,
         auth: Auth,
         frontend_config: FrontendConfig,
         lab: Lab,
     ) -> None:
-        super().__init__(app)
+        super().__init__(app, auth)
 
-        router = APIRouter()
-        self.prefix_dir, federated_extensions = lab.init_router(router, "lab")
-        extensions_dir = self.prefix_dir / "share" / "jupyter" / "labextensions"
+        self.jupyterlab_config = jupyterlab_config
+        self.frontend_config = frontend_config
+        self.lab = lab
+        lab.redirect_after_root = "lab"
+
+        extensions_dir = lab.prefix_dir / "share" / "jupyter" / "labextensions"
         self.federated_extensions, self.disabled_extension = lab.get_federated_extensions(
             extensions_dir
         )
         jupyterlab_dir = Path(jupyterlab_module.__file__).parents[1]
 
         if jupyterlab_config.dev_mode:
             self.static_lab_dir = jupyterlab_dir / "dev_mode" / "static"
         else:
-            self.static_lab_dir = self.prefix_dir / "share" / "jupyter" / "lab" / "static"
+            self.static_lab_dir = lab.prefix_dir / "share" / "jupyter" / "lab" / "static"
 
         self.mount(
             "/static/lab",
             StaticFiles(directory=self.static_lab_dir),
             name="static",
         )
 
-        @router.get("/lab")
-        async def get_lab(
-            user: User = Depends(auth.current_user()),
-        ):
-            return HTMLResponse(
-                self.get_index(
-                    "default",
-                    frontend_config.collaborative,
-                    jupyterlab_config.dev_mode,
-                    frontend_config.base_url,
-                )
+    async def get_lab(
+        self,
+        user: User,
+    ):
+        return HTMLResponse(
+            self.get_index(
+                "default",
+                self.frontend_config.collaborative,
+                self.jupyterlab_config.dev_mode,
+                self.frontend_config.base_url,
             )
+        )
 
-        @router.get("/lab/tree/{path:path}")
-        async def load_workspace(
-            path,
-        ):
-            return HTMLResponse(
-                self.get_index(
-                    "default",
-                    frontend_config.collaborative,
-                    jupyterlab_config.dev_mode,
-                    frontend_config.base_url,
-                )
+    async def load_workspace(
+        self,
+        path,
+    ):
+        return HTMLResponse(
+            self.get_index(
+                "default",
+                self.frontend_config.collaborative,
+                self.jupyterlab_config.dev_mode,
+                self.frontend_config.base_url,
             )
-
-        @router.get("/lab/api/workspaces/{name}")
-        async def get_workspace_data(user: User = Depends(auth.current_user())):
-            if user:
-                return json.loads(user.workspace)
-            return {}
-
-        @router.put(
-            "/lab/api/workspaces/{name}",
-            status_code=204,
         )
-        async def set_workspace(
-            request: Request,
-            user: User = Depends(auth.current_user()),
-            user_update=Depends(auth.update_user),
-        ):
-            workspace = (await request.body()).decode("utf-8")
-            await user_update({"workspace": workspace})
-            return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
-        @router.get("/lab/workspaces/{name}", response_class=HTMLResponse)
-        async def get_workspace(
-            name,
-            user: User = Depends(auth.current_user()),
-        ):
-            return self.get_index(
-                name,
-                frontend_config.collaborative,
-                jupyterlab_config.dev_mode,
-                frontend_config.base_url,
-            )
+    async def get_workspace_data(self, user: User):
+        if user:
+            return json.loads(user.workspace)
+        return {}
+
+    async def set_workspace(
+        self,
+        request: Request,
+        user: User,
+        user_update,
+    ):
+        workspace = (await request.body()).decode("utf-8")
+        await user_update({"workspace": workspace})
+        return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
-        self.include_router(router)
+    async def get_workspace(
+        self,
+        name,
+        user: User,
+    ):
+        return self.get_index(
+            name,
+            self.frontend_config.collaborative,
+            self.jupyterlab_config.dev_mode,
+            self.frontend_config.base_url,
+        )
 
     def get_index(self, workspace, collaborative, dev_mode, base_url="/"):
         for path in (self.static_lab_dir).glob("main.*.js"):
             main_id = path.name.split(".")[1]
             break
         vendor_id = None
         for path in (self.static_lab_dir).glob("vendors-node_modules_whatwg-fetch_fetch_js.*.js"):
@@ -145,17 +142,19 @@
             "listingsUrl": "/lab/api/listings",
             "mathjaxConfig": "TeX-AMS-MML_HTMLorMML-full,Safe",
             "mode": "multiple-document",
             "notebookVersion": "[1, 9, 0]",
             "quitButton": True,
             "settingsUrl": "/lab/api/settings",
             "store_id": 0,
-            "schemasDir": (self.prefix_dir / "share" / "jupyter" / "lab" / "schemas").as_posix(),
+            "schemasDir": (
+                self.lab.prefix_dir / "share" / "jupyter" / "lab" / "schemas"
+            ).as_posix(),
             "terminalsAvailable": True,
-            "themesDir": (self.prefix_dir / "share" / "jupyter" / "lab" / "themes").as_posix(),
+            "themesDir": (self.lab.prefix_dir / "share" / "jupyter" / "lab" / "themes").as_posix(),
             "themesUrl": "/lab/api/themes",
             "token": "4e2804532de366abc81e32ab0c6bf68a73716fafbdbb2098",
             "translationsApiUrl": "/lab/api/translations",
             "treePath": "",
             "workspace": workspace,
             "treeUrl": "/lab/tree",
             "workspacesApiUrl": "/lab/api/workspaces",
```

### Comparing `fps_jupyterlab-0.1.3/.gitignore` & `fps_jupyterlab-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_jupyterlab-0.1.3/COPYING.md` & `fps_jupyterlab-0.1.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_jupyterlab-0.1.3/pyproject.toml` & `fps_jupyterlab-0.1.4/pyproject.toml`

 * *Files identical despite different names*


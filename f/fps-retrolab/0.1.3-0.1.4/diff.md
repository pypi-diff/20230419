# Comparing `tmp/fps_retrolab-0.1.3.tar.gz` & `tmp/fps_retrolab-0.1.4.tar.gz`

## Comparing `fps_retrolab-0.1.3.tar` & `fps_retrolab-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_retrolab-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_retrolab-0.1.3/fps_retrolab/__init__.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 fps_retrolab-0.1.3/fps_retrolab/main.py
--rw-r--r--   0        0        0     6717 2020-02-02 00:00:00.000000 fps_retrolab-0.1.3/fps_retrolab/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_retrolab-0.1.3/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_retrolab-0.1.3/COPYING.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fps_retrolab-0.1.3/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 fps_retrolab-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fps_retrolab-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_retrolab-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_retrolab-0.1.4/fps_retrolab/__init__.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 fps_retrolab-0.1.4/fps_retrolab/main.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 fps_retrolab-0.1.4/fps_retrolab/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_retrolab-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_retrolab-0.1.4/COPYING.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fps_retrolab-0.1.4/README.md
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 fps_retrolab-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 fps_retrolab-0.1.4/PKG-INFO
```

### Comparing `fps_retrolab-0.1.3/fps_retrolab/main.py` & `fps_retrolab-0.1.4/fps_retrolab/main.py`

 * *Files identical despite different names*

### Comparing `fps_retrolab-0.1.3/fps_retrolab/routes.py` & `fps_retrolab-0.1.4/fps_retrolab/routes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,147 +1,120 @@
 import json
 from pathlib import Path
 
 import retrolab  # type: ignore
-from fastapi import APIRouter, Depends
-from fastapi.responses import HTMLResponse
 from fastapi.staticfiles import StaticFiles
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.frontend import FrontendConfig
 from jupyverse_api.lab import Lab
 from jupyverse_api.retrolab import RetroLab
 
 
 class _RetroLab(RetroLab):
     def __init__(self, app: App, auth: Auth, frontend_config: FrontendConfig, lab: Lab) -> None:
-        super().__init__(app)
+        super().__init__(app, auth, lab)
+        self.frontend_config = frontend_config
+        self.lab = lab
+        self.lab.redirect_after_root = "retro/tree"
 
-        router = APIRouter()
-        prefix_dir, federated_extensions = lab.init_router(router, "retro/tree")
-        retrolab_dir = Path(retrolab.__file__).parent
+        self.retrolab_dir = Path(retrolab.__file__).parent
 
         self.mount(
             "/static/retro",
-            StaticFiles(directory=retrolab_dir / "static"),
+            StaticFiles(directory=self.retrolab_dir / "static"),
             name="static",
         )
 
-        for path in (retrolab_dir / "labextension" / "static").glob("remoteEntry.*.js"):
+        for path in (self.retrolab_dir / "labextension" / "static").glob("remoteEntry.*.js"):
             load = f"static/{path.name}"
             break
-        retro_federated_extensions = [
+
+        self.retro_federated_extensions = [
             {
                 "extension": "./extension",
                 "load": load,
                 "name": "@retrolab/lab-extension",
                 "style": "./style",
             }
         ]
 
-        @router.get("/retro/tree", response_class=HTMLResponse)
-        async def get_tree(
-            user: User = Depends(auth.current_user()),
-        ):
-            return get_index(
-                "Tree", "tree", frontend_config.collaborative, frontend_config.base_url
-            )
+    async def get_tree(
+        self,
+        user: User,
+    ):
+        return get_index(
+            self.lab,
+            self.retrolab_dir,
+            self.retro_federated_extensions,
+            "Tree",
+            "tree",
+            self.frontend_config.collaborative,
+            self.frontend_config.base_url,
+        )
 
-        @router.get("/retro/notebooks/{path:path}", response_class=HTMLResponse)
-        async def get_notebook(
+    async def get_notebook(
+        self,
+        path,
+        user: User,
+    ):
+        return get_index(
+            self.lab,
+            self.retrolab_dir,
+            self.retro_federated_extensions,
             path,
-            user: User = Depends(auth.current_user()),
-        ):
-            return get_index(
-                path, "notebooks", frontend_config.collaborative, frontend_config.base_url
-            )
+            "notebooks",
+            self.frontend_config.collaborative,
+            self.frontend_config.base_url,
+        )
 
-        @router.get("/retro/edit/{path:path}", response_class=HTMLResponse)
-        async def edit_file(
+    async def edit_file(
+        self,
+        path,
+        user: User,
+    ):
+        return get_index(
+            self.lab,
+            self.retrolab_dir,
+            self.retro_federated_extensions,
             path,
-            user: User = Depends(auth.current_user()),
-        ):
-            return get_index(path, "edit", frontend_config.collaborative, frontend_config.base_url)
+            "edit",
+            self.frontend_config.collaborative,
+            self.frontend_config.base_url,
+        )
 
-        @router.get("/retro/consoles/{path:path}", response_class=HTMLResponse)
-        async def get_console(
+    async def get_console(
+        self,
+        path,
+        user: User,
+    ):
+        return get_index(
+            self.lab,
+            self.retrolab_dir,
+            self.retro_federated_extensions,
             path,
-            user: User = Depends(auth.current_user()),
-        ):
-            return get_index(
-                path, "consoles", frontend_config.collaborative, frontend_config.base_url
-            )
-
-        @router.get("/retro/terminals/{name}", response_class=HTMLResponse)
-        async def get_terminal(
-            name: str,
-            user: User = Depends(auth.current_user()),
-        ):
-            return get_index(
-                name, "terminals", frontend_config.collaborative, frontend_config.base_url
-            )
-
-        def get_index(doc_name, retro_page, collaborative, base_url="/"):
-            extensions_dir = prefix_dir / "share" / "jupyter" / "labextensions"
-            federated_extensions, disabled_extension = lab.get_federated_extensions(extensions_dir)
-            page_config = {
-                "appName": "RetroLab",
-                "appNamespace": "retro",
-                "appSettingsDir": (
-                    prefix_dir / "share" / "jupyter" / "lab" / "settings"
-                ).as_posix(),
-                "appUrl": "/lab",
-                "appVersion": retrolab.__version__,
-                "baseUrl": base_url,
-                "cacheFiles": True,
-                "collaborative": collaborative,
-                "disabledExtensions": disabled_extension,
-                "extraLabextensionsPath": [],
-                "federated_extensions": retro_federated_extensions + federated_extensions,
-                "frontendUrl": "/retro/",
-                "fullAppUrl": f"{base_url}lab",
-                "fullLabextensionsUrl": f"{base_url}lab/extensions",
-                "fullLicensesUrl": f"{base_url}lab/api/licenses",
-                "fullListingsUrl": f"{base_url}lab/api/listings",
-                "fullMathjaxUrl": f"{base_url}static/notebook/components/MathJax/MathJax.js",
-                "fullSettingsUrl": f"{base_url}lab/api/settings",
-                "fullStaticUrl": f"{base_url}static/retro",
-                "fullThemesUrl": f"{base_url}lab/api/themes",
-                "fullTranslationsApiUrl": f"{base_url}lab/api/translations",
-                "fullTreeUrl": f"{base_url}lab/tree",
-                "fullWorkspacesApiUrl": f"{base_url}lab/api/workspaces",
-                "labextensionsPath": [
-                    (prefix_dir / "share" / "jupyter" / "labextensions").as_posix()
-                ],
-                "labextensionsUrl": "/lab/extensions",
-                "licensesUrl": "/lab/api/licenses",
-                "listingsUrl": "/lab/api/listings",
-                "mathjaxConfig": "TeX-AMS-MML_HTMLorMML-full,Safe",
-                "retroLogo": False,
-                "retroPage": retro_page,
-                "schemasDir": (prefix_dir / "share" / "jupyter" / "lab" / "schemas").as_posix(),
-                "settingsUrl": "/lab/api/settings",
-                "staticDir": (retrolab_dir / "static").as_posix(),
-                "templatesDir": (retrolab_dir / "templates").as_posix(),
-                "terminalsAvailable": True,
-                "themesDir": (prefix_dir / "share" / "jupyter" / "lab" / "themes").as_posix(),
-                "themesUrl": "/lab/api/themes",
-                "translationsApiUrl": "/lab/api/translations",
-                "treeUrl": "/lab/tree",
-                "workspacesApiUrl": "/lab/api/workspaces",
-                "wsUrl": "",
-            }
-            index = (
-                INDEX_HTML.replace("PAGE_CONFIG", json.dumps(page_config))
-                .replace("DOC_NAME", doc_name)
-                .replace("BASE_URL", base_url)
-            )
-            return index
+            "consoles",
+            self.frontend_config.collaborative,
+            self.frontend_config.base_url,
+        )
 
-        self.include_router(router)
+    async def get_terminal(
+        self,
+        name: str,
+        user: User,
+    ):
+        return get_index(
+            self.lab,
+            self.retrolab_dir,
+            self.retro_federated_extensions,
+            name,
+            "terminals",
+            self.frontend_config.collaborative,
+            self.frontend_config.base_url,
+        )
 
 
 INDEX_HTML = """\
 <!DOCTYPE html>
 <html>
 <head>
   <meta charset="utf-8">
@@ -164,7 +137,63 @@
         window.history.replaceState({ }, '', parsedUrl.href);
       }
     })();
   </script>
 </body>
 </html>
 """
+
+
+def get_index(
+    lab, retrolab_dir, retro_federated_extensions, doc_name, retro_page, collaborative, base_url="/"
+):
+    extensions_dir = lab.prefix_dir / "share" / "jupyter" / "labextensions"
+    federated_extensions, disabled_extension = lab.get_federated_extensions(extensions_dir)
+    page_config = {
+        "appName": "RetroLab",
+        "appNamespace": "retro",
+        "appSettingsDir": (lab.prefix_dir / "share" / "jupyter" / "lab" / "settings").as_posix(),
+        "appUrl": "/lab",
+        "appVersion": retrolab.__version__,
+        "baseUrl": base_url,
+        "cacheFiles": True,
+        "collaborative": collaborative,
+        "disabledExtensions": disabled_extension,
+        "extraLabextensionsPath": [],
+        "federated_extensions": retro_federated_extensions + federated_extensions,
+        "frontendUrl": "/retro/",
+        "fullAppUrl": f"{base_url}lab",
+        "fullLabextensionsUrl": f"{base_url}lab/extensions",
+        "fullLicensesUrl": f"{base_url}lab/api/licenses",
+        "fullListingsUrl": f"{base_url}lab/api/listings",
+        "fullMathjaxUrl": f"{base_url}static/notebook/components/MathJax/MathJax.js",
+        "fullSettingsUrl": f"{base_url}lab/api/settings",
+        "fullStaticUrl": f"{base_url}static/retro",
+        "fullThemesUrl": f"{base_url}lab/api/themes",
+        "fullTranslationsApiUrl": f"{base_url}lab/api/translations",
+        "fullTreeUrl": f"{base_url}lab/tree",
+        "fullWorkspacesApiUrl": f"{base_url}lab/api/workspaces",
+        "labextensionsPath": [(lab.prefix_dir / "share" / "jupyter" / "labextensions").as_posix()],
+        "labextensionsUrl": "/lab/extensions",
+        "licensesUrl": "/lab/api/licenses",
+        "listingsUrl": "/lab/api/listings",
+        "mathjaxConfig": "TeX-AMS-MML_HTMLorMML-full,Safe",
+        "retroLogo": False,
+        "retroPage": retro_page,
+        "schemasDir": (lab.prefix_dir / "share" / "jupyter" / "lab" / "schemas").as_posix(),
+        "settingsUrl": "/lab/api/settings",
+        "staticDir": (retrolab_dir / "static").as_posix(),
+        "templatesDir": (retrolab_dir / "templates").as_posix(),
+        "terminalsAvailable": True,
+        "themesDir": (lab.prefix_dir / "share" / "jupyter" / "lab" / "themes").as_posix(),
+        "themesUrl": "/lab/api/themes",
+        "translationsApiUrl": "/lab/api/translations",
+        "treeUrl": "/lab/tree",
+        "workspacesApiUrl": "/lab/api/workspaces",
+        "wsUrl": "",
+    }
+    index = (
+        INDEX_HTML.replace("PAGE_CONFIG", json.dumps(page_config))
+        .replace("DOC_NAME", doc_name)
+        .replace("BASE_URL", base_url)
+    )
+    return index
```

### Comparing `fps_retrolab-0.1.3/.gitignore` & `fps_retrolab-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_retrolab-0.1.3/COPYING.md` & `fps_retrolab-0.1.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_retrolab-0.1.3/pyproject.toml` & `fps_retrolab-0.1.4/pyproject.toml`

 * *Files identical despite different names*


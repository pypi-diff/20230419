# Comparing `tmp/fps_nbconvert-0.1.3.tar.gz` & `tmp/fps_nbconvert-0.1.4.tar.gz`

## Comparing `fps_nbconvert-0.1.3.tar` & `fps_nbconvert-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.3/fps_nbconvert/__init__.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.3/fps_nbconvert/main.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.3/fps_nbconvert/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.3/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.3/COPYING.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.3/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.4/fps_nbconvert/__init__.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.4/fps_nbconvert/main.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.4/fps_nbconvert/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.4/COPYING.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.4/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 fps_nbconvert-0.1.4/PKG-INFO
```

### Comparing `fps_nbconvert-0.1.3/fps_nbconvert/routes.py` & `fps_nbconvert-0.1.4/fps_nbconvert/routes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 import tempfile
 from pathlib import Path
 
 import nbconvert
-from fastapi import APIRouter, Depends
 from fastapi.responses import FileResponse
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.nbconvert import Nbconvert
 
 
 class _Nbconvert(Nbconvert):
     def __init__(
         self,
         app: App,
         auth: Auth,
     ) -> None:
-        super().__init__(app)
+        super().__init__(app, auth)
 
-        router = APIRouter()
+    async def get_nbconvert_formats(self):
+        return {
+            name: {"output_mimetype": nbconvert.exporters.get_exporter(name).output_mimetype}
+            for name in nbconvert.exporters.get_export_names()
+        }
 
-        @router.get("/api/nbconvert")
-        async def get_nbconvert_formats():
-            return {
-                name: {"output_mimetype": nbconvert.exporters.get_exporter(name).output_mimetype}
-                for name in nbconvert.exporters.get_export_names()
-            }
-
-        @router.get("/nbconvert/{format}/{path}")
-        async def get_nbconvert_document(
-            format: str,
-            path: str,
-            download: bool,
-            user: User = Depends(auth.current_user(permissions={"nbconvert": ["read"]})),
-        ):
-            exporter = nbconvert.exporters.get_exporter(format)
-            if download:
-                media_type = "application/octet-stream"
-            else:
-                media_type = exporter.output_mimetype
-            tmp_dir = Path(tempfile.mkdtemp())
-            tmp_path = tmp_dir / (Path(path).stem + exporter().file_extension)
-            with open(tmp_path, "wt") as f:
-                f.write(exporter().from_filename(path)[0])
-            return FileResponse(tmp_path, media_type=media_type, filename=tmp_path.name)
-
-        self.include_router(router)
+    async def get_nbconvert_document(
+        self,
+        format: str,
+        path: str,
+        download: bool,
+        user: User,
+    ):
+        exporter = nbconvert.exporters.get_exporter(format)
+        if download:
+            media_type = "application/octet-stream"
+        else:
+            media_type = exporter.output_mimetype
+        tmp_dir = Path(tempfile.mkdtemp())
+        tmp_path = tmp_dir / (Path(path).stem + exporter().file_extension)
+        with open(tmp_path, "wt") as f:
+            f.write(exporter().from_filename(path)[0])
+        return FileResponse(tmp_path, media_type=media_type, filename=tmp_path.name)
```

### Comparing `fps_nbconvert-0.1.3/.gitignore` & `fps_nbconvert-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_nbconvert-0.1.3/COPYING.md` & `fps_nbconvert-0.1.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_nbconvert-0.1.3/pyproject.toml` & `fps_nbconvert-0.1.4/pyproject.toml`

 * *Files identical despite different names*


# Comparing `tmp/fps_contents-0.1.3.tar.gz` & `tmp/fps_contents-0.1.4.tar.gz`

## Comparing `fps_contents-0.1.3.tar` & `fps_contents-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_contents-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_contents-0.1.3/fps_contents/__init__.py
--rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 fps_contents-0.1.3/fps_contents/fileid.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 fps_contents-0.1.3/fps_contents/main.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 fps_contents-0.1.3/fps_contents/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_contents-0.1.3/fps_contents/py.typed
--rw-r--r--   0        0        0    10716 2020-02-02 00:00:00.000000 fps_contents-0.1.3/fps_contents/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_contents-0.1.3/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_contents-0.1.3/COPYING.md
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fps_contents-0.1.3/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fps_contents-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fps_contents-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_contents-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_contents-0.1.4/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8386 2020-02-02 00:00:00.000000 fps_contents-0.1.4/fps_contents/fileid.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 fps_contents-0.1.4/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_contents-0.1.4/fps_contents/py.typed
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 fps_contents-0.1.4/fps_contents/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_contents-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_contents-0.1.4/COPYING.md
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 fps_contents-0.1.4/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 fps_contents-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 fps_contents-0.1.4/PKG-INFO
```

### Comparing `fps_contents-0.1.3/fps_contents/fileid.py` & `fps_contents-0.1.4/fps_contents/fileid.py`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.3/fps_contents/routes.py` & `fps_contents-0.1.4/fps_contents/routes.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,157 +3,142 @@
 import shutil
 from datetime import datetime
 from http import HTTPStatus
 from pathlib import Path
 from typing import Dict, List, Optional, Union, cast
 
 from anyio import open_file
-from fastapi import APIRouter, Depends, HTTPException, Response
-from jupyverse_api.app import App
-from jupyverse_api.auth import Auth, User
-from jupyverse_api.contents import Contents, Content, SaveContent
+from fastapi import HTTPException, Response
+from jupyverse_api.auth import User
+from jupyverse_api.contents import Contents
+from jupyverse_api.contents.models import (
+    Checkpoint,
+    Content,
+    CreateContent,
+    RenameContent,
+    SaveContent,
+)
 from starlette.requests import Request
 
 from .fileid import FileIdManager
-from .models import Checkpoint, CreateContent, RenameContent
 
 
 class _Contents(Contents):
-    def __init__(self, app: App, auth: Auth):
-        super().__init__(app=app)
-
-        router = APIRouter()
-
-        @router.post(
-            "/api/contents/{path:path}/checkpoints",
-            status_code=201,
-        )
-        async def create_checkpoint(
-            path, user: User = Depends(auth.current_user(permissions={"contents": ["write"]}))
-        ):
-            src_path = Path(path)
+    async def create_checkpoint(
+        self,
+        path,
+        user: User,
+    ):
+        src_path = Path(path)
+        dst_path = Path(".ipynb_checkpoints") / f"{src_path.stem}-checkpoint{src_path.suffix}"
+        try:
+            dst_path.parent.mkdir(exist_ok=True)
+            shutil.copyfile(src_path, dst_path)
+        except Exception:
+            # FIXME: return error code?
+            return []
+        mtime = get_file_modification_time(dst_path)
+        return Checkpoint(**{"id": "checkpoint", "last_modified": mtime})
+
+    async def create_content(
+        self,
+        path: Optional[str],
+        request: Request,
+        user: User,
+    ):
+        create_content = CreateContent(**(await request.json()))
+        content_path = Path(create_content.path)
+        if create_content.type == "notebook":
+            available_path = get_available_path(content_path / "Untitled.ipynb")
+            async with await open_file(available_path, "w") as f:
+                await f.write(
+                    json.dumps({"cells": [], "metadata": {}, "nbformat": 4, "nbformat_minor": 5})
+                )
+            src_path = available_path
             dst_path = Path(".ipynb_checkpoints") / f"{src_path.stem}-checkpoint{src_path.suffix}"
             try:
                 dst_path.parent.mkdir(exist_ok=True)
                 shutil.copyfile(src_path, dst_path)
             except Exception:
                 # FIXME: return error code?
-                return []
-            mtime = get_file_modification_time(dst_path)
-            return Checkpoint(**{"id": "checkpoint", "last_modified": mtime})
-
-        @router.post(
-            "/api/contents{path:path}",
-            status_code=201,
-        )
-        async def create_content(
-            path: Optional[str],
-            request: Request,
-            user: User = Depends(auth.current_user(permissions={"contents": ["write"]})),
-        ):
-            create_content = CreateContent(**(await request.json()))
-            content_path = Path(create_content.path)
-            if create_content.type == "notebook":
-                available_path = get_available_path(content_path / "Untitled.ipynb")
-                async with await open_file(available_path, "w") as f:
-                    await f.write(
-                        json.dumps(
-                            {"cells": [], "metadata": {}, "nbformat": 4, "nbformat_minor": 5}
-                        )
-                    )
-                src_path = available_path
-                dst_path = (
-                    Path(".ipynb_checkpoints") / f"{src_path.stem}-checkpoint{src_path.suffix}"
-                )
-                try:
-                    dst_path.parent.mkdir(exist_ok=True)
-                    shutil.copyfile(src_path, dst_path)
-                except Exception:
-                    # FIXME: return error code?
-                    pass
-            elif create_content.type == "directory":
-                name = "Untitled Folder"
-                available_path = get_available_path(content_path / name, sep=" ")
-                available_path.mkdir(parents=True, exist_ok=True)
+                pass
+        elif create_content.type == "directory":
+            name = "Untitled Folder"
+            available_path = get_available_path(content_path / name, sep=" ")
+            available_path.mkdir(parents=True, exist_ok=True)
+        else:
+            assert create_content.ext is not None
+            available_path = get_available_path(content_path / ("untitled" + create_content.ext))
+            open(available_path, "w").close()
+
+        return await self.read_content(available_path, False)
+
+    async def get_root_content(
+        self,
+        content: int,
+        user: User,
+    ):
+        return await self.read_content("", bool(content))
+
+    async def get_checkpoint(
+        self,
+        path,
+        user: User,
+    ):
+        src_path = Path(path)
+        dst_path = Path(".ipynb_checkpoints") / f"{src_path.stem}-checkpoint{src_path.suffix}"
+        if not dst_path.exists():
+            return []
+        mtime = get_file_modification_time(dst_path)
+        return [Checkpoint(**{"id": "checkpoint", "last_modified": mtime})]
+
+    async def get_content(
+        self,
+        path: str,
+        content: int,
+        user: User,
+    ):
+        return await self.read_content(path, bool(content))
+
+    async def save_content(
+        self,
+        path,
+        request: Request,
+        response: Response,
+        user: User,
+    ):
+        content = SaveContent(**(await request.json()))
+        try:
+            await self.write_content(content)
+        except Exception:
+            raise HTTPException(status_code=404, detail=f"Error saving {content.path}")
+        return await self.read_content(content.path, False)
+
+    async def delete_content(
+        self,
+        path,
+        user: User,
+    ):
+        p = Path(path)
+        if p.exists():
+            if p.is_dir():
+                shutil.rmtree(p)
             else:
-                assert create_content.ext is not None
-                available_path = get_available_path(
-                    content_path / ("untitled" + create_content.ext)
-                )
-                open(available_path, "w").close()
-
-            return await self.read_content(available_path, False)
-
-        @router.get("/api/contents")
-        async def get_root_content(
-            content: int,
-            user: User = Depends(auth.current_user(permissions={"contents": ["read"]})),
-        ):
-            return await self.read_content("", bool(content))
-
-        @router.get("/api/contents/{path:path}/checkpoints")
-        async def get_checkpoint(
-            path, user: User = Depends(auth.current_user(permissions={"contents": ["read"]}))
-        ):
-            src_path = Path(path)
-            dst_path = Path(".ipynb_checkpoints") / f"{src_path.stem}-checkpoint{src_path.suffix}"
-            if not dst_path.exists():
-                return []
-            mtime = get_file_modification_time(dst_path)
-            return [Checkpoint(**{"id": "checkpoint", "last_modified": mtime})]
-
-        @router.get("/api/contents/{path:path}")
-        async def get_content(
-            path: str,
-            content: int = 0,
-            user: User = Depends(auth.current_user(permissions={"contents": ["read"]})),
-        ):
-            return await self.read_content(path, bool(content))
-
-        @router.put("/api/contents/{path:path}")
-        async def save_content(
-            path,
-            request: Request,
-            response: Response,
-            user: User = Depends(auth.current_user(permissions={"contents": ["write"]})),
-        ):
-            content = SaveContent(**(await request.json()))
-            try:
-                await self.write_content(content)
-            except Exception:
-                raise HTTPException(status_code=404, detail=f"Error saving {content.path}")
-            return await self.read_content(content.path, False)
-
-        @router.delete(
-            "/api/contents/{path:path}",
-            status_code=204,
-        )
-        async def delete_content(
-            path,
-            user: User = Depends(auth.current_user(permissions={"contents": ["write"]})),
-        ):
-            p = Path(path)
-            if p.exists():
-                if p.is_dir():
-                    shutil.rmtree(p)
-                else:
-                    p.unlink()
-            return Response(status_code=HTTPStatus.NO_CONTENT.value)
-
-        @router.patch("/api/contents/{path:path}")
-        async def rename_content(
-            path,
-            request: Request,
-            user: User = Depends(auth.current_user(permissions={"contents": ["write"]})),
-        ):
-            rename_content = RenameContent(**(await request.json()))
-            Path(path).rename(rename_content.path)
-            return await self.read_content(rename_content.path, False)
+                p.unlink()
+        return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
-        self.include_router(router)
+    async def rename_content(
+        self,
+        path,
+        request: Request,
+        user: User,
+    ):
+        rename_content = RenameContent(**(await request.json()))
+        Path(path).rename(rename_content.path)
+        return await self.read_content(rename_content.path, False)
 
     async def read_content(
         self, path: Union[str, Path], get_content: bool, as_json: bool = False
     ) -> Content:
         if isinstance(path, str):
             path = Path(path)
         content: Optional[Union[str, Dict, List[Dict]]] = None
```

### Comparing `fps_contents-0.1.3/.gitignore` & `fps_contents-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.3/COPYING.md` & `fps_contents-0.1.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.3/pyproject.toml` & `fps_contents-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_contents-0.1.3/PKG-INFO` & `fps_contents-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_contents
-Version: 0.1.3
+Version: 0.1.4
 Summary: An FPS plugin for the contents API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```


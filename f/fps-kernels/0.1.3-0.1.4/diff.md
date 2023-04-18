# Comparing `tmp/fps_kernels-0.1.3.tar.gz` & `tmp/fps_kernels-0.1.4.tar.gz`

## Comparing `fps_kernels-0.1.3.tar` & `fps_kernels-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/fps_kernels/main.py
--rw-r--r--   0        0        0    15262 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/COPYING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fps_kernels-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/main.py
+-rw-r--r--   0        0        0    13051 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4078 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/COPYING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fps_kernels-0.1.4/PKG-INFO
```

### Comparing `fps_kernels-0.1.3/fps_kernels/main.py` & `fps_kernels-0.1.4/fps_kernels/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,15 +29,19 @@
         ctx: Context,
     ) -> AsyncGenerator[None, Optional[BaseException]]:
         ctx.add_resource(self.kernels_config, types=KernelsConfig)
 
         app = await ctx.request_resource(App)
         auth = await ctx.request_resource(Auth)  # type: ignore
         frontend_config = await ctx.request_resource(FrontendConfig)
-        yjs = await ctx.request_resource(Yjs)
+        yjs = (
+            await ctx.request_resource(Yjs)  # type: ignore
+            if self.kernels_config.require_yjs
+            else None
+        )
 
         kernels = _Kernels(app, self.kernels_config, auth, frontend_config, yjs)
         ctx.add_resource(kernels, types=Kernels)
 
         if self.kernels_config.connection_path is not None:
             path = Path(self.kernels_config.connection_path)
             task = asyncio.create_task(kernels.watch_connection_files(path))
```

### Comparing `fps_kernels-0.1.3/fps_kernels/routes.py` & `fps_kernels-0.1.4/fps_kernels/routes.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
-import sys
 import uuid
 from http import HTTPStatus
 from pathlib import Path
-from typing import Dict, List, Set, Tuple
+from typing import Dict, List, Optional, Set, Tuple
 
-from fastapi import APIRouter, Depends, HTTPException, Response
+from fastapi import HTTPException, Response
 from fastapi.responses import FileResponse
 from starlette.requests import Request
 from watchfiles import Change, awatch
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.kernels import Kernels, KernelsConfig
 from jupyverse_api.kernels.models import CreateSession, Execution, Kernel, Notebook, Session
 from jupyverse_api.frontend import FrontendConfig
@@ -28,294 +27,287 @@
 class _Kernels(Kernels):
     def __init__(
         self,
         app: App,
         kernels_config: KernelsConfig,
         auth: Auth,
         frontend_config: FrontendConfig,
-        yjs: Yjs,
+        yjs: Optional[Yjs],
     ) -> None:
-        super().__init__(app)
+        super().__init__(app=app, auth=auth)
+        self.kernels_config = kernels_config
+        self.frontend_config = frontend_config
+        self.yjs = yjs
 
-        router = APIRouter()
-
-        kernelspecs: dict = {}
+        self.kernelspecs: dict = {}
         self.kernel_id_to_connection_file: Dict[str, str] = {}
-        sessions: Dict[str, Session] = {}
-        Path(sys.prefix)
+        self.sessions: Dict[str, Session] = {}
+        self.kernels = kernels
 
-        @router.get("/api/kernelspecs")
-        async def get_kernelspecs(
-            user: User = Depends(auth.current_user(permissions={"kernelspecs": ["read"]})),
-        ):
-            for search_path in kernelspec_dirs():
-                for path in Path(search_path).glob("*/kernel.json"):
-                    with open(path) as f:
-                        spec = json.load(f)
-                    name = path.parent.name
-                    resources = {
-                        f.stem: f"{frontend_config.base_url}kernelspecs/{name}/{f.name}"
-                        for f in path.parent.iterdir()
-                        if f.is_file() and f.name != "kernel.json"
-                    }
-                    kernelspecs[name] = {"name": name, "spec": spec, "resources": resources}
-            return {"default": kernels_config.default_kernel, "kernelspecs": kernelspecs}
-
-        @router.get("/kernelspecs/{kernel_name}/{file_name}")
-        async def get_kernelspec(
-            kernel_name,
-            file_name,
-            user: User = Depends(auth.current_user()),
-        ):
-            for search_path in kernelspec_dirs():
-                file_path = Path(search_path) / kernel_name / file_name
-                if file_path.exists():
-                    return FileResponse(file_path)
-            raise HTTPException(
-                status_code=404, detail=f"Kernelspec {kernel_name}/{file_name} not found"
-            )
+    async def get_kernelspecs(
+        self,
+        user: User,
+    ):
+        for search_path in kernelspec_dirs():
+            for path in Path(search_path).glob("*/kernel.json"):
+                with open(path) as f:
+                    spec = json.load(f)
+                name = path.parent.name
+                resources = {
+                    f.stem: f"{self.frontend_config.base_url}kernelspecs/{name}/{f.name}"
+                    for f in path.parent.iterdir()
+                    if f.is_file() and f.name != "kernel.json"
+                }
+                self.kernelspecs[name] = {"name": name, "spec": spec, "resources": resources}
+        return {"default": self.kernels_config.default_kernel, "kernelspecs": self.kernelspecs}
 
-        @router.get("/api/kernels")
-        async def get_kernels(
-            user: User = Depends(auth.current_user(permissions={"kernels": ["read"]})),
-        ):
-            results = []
-            for kernel_id, kernel in kernels.items():
-                if kernel["server"]:
-                    connections = kernel["server"].connections
-                    last_activity = kernel["server"].last_activity["date"]
-                    execution_state = kernel["server"].last_activity["execution_state"]
-                else:
-                    connections = 0
-                    last_activity = ""
-                    execution_state = "idle"
-                results.append(
-                    {
-                        "id": kernel_id,
-                        "name": kernel["name"],
-                        "connections": connections,
-                        "last_activity": last_activity,
-                        "execution_state": execution_state,
-                    }
-                )
-            return results
+    async def get_kernelspec(
+        self,
+        kernel_name,
+        file_name,
+        user: User,
+    ):
+        for search_path in kernelspec_dirs():
+            file_path = Path(search_path) / kernel_name / file_name
+            if file_path.exists():
+                return FileResponse(file_path)
 
-        @router.delete("/api/sessions/{session_id}", status_code=204)
-        async def delete_session(
-            session_id: str,
-            user: User = Depends(auth.current_user(permissions={"sessions": ["write"]})),
-        ):
-            kernel_id = sessions[session_id].kernel.id
-            kernel_server = kernels[kernel_id]["server"]
-            await kernel_server.stop()
-            del kernels[kernel_id]
-            if kernel_id in self.kernel_id_to_connection_file:
-                del self.kernel_id_to_connection_file[kernel_id]
-            del sessions[session_id]
-            return Response(status_code=HTTPStatus.NO_CONTENT.value)
-
-        @router.patch("/api/sessions/{session_id}")
-        async def rename_session(
-            request: Request,
-            user: User = Depends(auth.current_user(permissions={"sessions": ["write"]})),
-        ):
-            rename_session = await request.json()
-            session_id = rename_session.pop("id")
-            for key, value in rename_session.items():
-                setattr(sessions[session_id], key, value)
-            return sessions[session_id]
-
-        @router.get("/api/sessions")
-        async def get_sessions(
-            user: User = Depends(auth.current_user(permissions={"sessions": ["read"]})),
-        ):
-            for session in sessions.values():
-                kernel_id = session.kernel.id
-                kernel_server = kernels[kernel_id]["server"]
-                session.kernel.last_activity = kernel_server.last_activity["date"]
-                session.kernel.execution_state = kernel_server.last_activity["execution_state"]
-            return list(sessions.values())
-
-        @router.post(
-            "/api/sessions",
-            status_code=201,
-            response_model=Session,
+        raise HTTPException(
+            status_code=404, detail=f"Kernelspec {kernel_name}/{file_name} not found"
         )
-        async def create_session(
-            request: Request,
-            user: User = Depends(auth.current_user(permissions={"sessions": ["write"]})),
-        ):
-            create_session = CreateSession(**(await request.json()))
-            kernel_id = create_session.kernel.id
-            kernel_name = create_session.kernel.name
-            if kernel_name is not None:
-                # launch a new ("internal") kernel
-                kernel_server = KernelServer(
-                    kernelspec_path=Path(find_kernelspec(kernel_name)).as_posix(),
-                    kernel_cwd=str(Path(create_session.path).parent),
-                )
-                kernel_id = str(uuid.uuid4())
-                kernels[kernel_id] = {"name": kernel_name, "server": kernel_server, "driver": None}
-                await kernel_server.start()
-            elif kernel_id is not None:
-                # external kernel
-                kernel_name = kernels[kernel_id]["name"]
-                kernel_server = KernelServer(
-                    connection_file=self.kernel_id_to_connection_file[kernel_id],
-                    write_connection_file=False,
-                )
-                kernels[kernel_id]["server"] = kernel_server
-                await kernel_server.start(launch_kernel=False)
-            else:
-                return
-            session_id = str(uuid.uuid4())
-            session = Session(
-                id=session_id,
-                path=create_session.path,
-                name=create_session.name,
-                type=create_session.type,
-                kernel=Kernel(
-                    id=kernel_id,
-                    name=kernel_name,
-                    connections=kernel_server.connections,
-                    last_activity=kernel_server.last_activity["date"],
-                    execution_state=kernel_server.last_activity["execution_state"],
-                ),
-                notebook=Notebook(
-                    path=create_session.path,
-                    name=create_session.name,
-                ),
-            )
-            sessions[session_id] = session
-            return session
 
-        @router.post("/api/kernels/{kernel_id}/interrupt")
-        async def interrupt_kernel(
-            kernel_id,
-            user: User = Depends(auth.current_user(permissions={"kernels": ["write"]})),
-        ):
-            if kernel_id in kernels:
-                kernel = kernels[kernel_id]
-                kernel["server"].interrupt()
-                result = {
+    async def get_kernels(
+        self,
+        user: User,
+    ):
+        results = []
+        for kernel_id, kernel in kernels.items():
+            if kernel["server"]:
+                connections = kernel["server"].connections
+                last_activity = kernel["server"].last_activity["date"]
+                execution_state = kernel["server"].last_activity["execution_state"]
+            else:
+                connections = 0
+                last_activity = ""
+                execution_state = "idle"
+            results.append(
+                {
                     "id": kernel_id,
                     "name": kernel["name"],
-                    "connections": kernel["server"].connections,
-                    "last_activity": kernel["server"].last_activity["date"],
-                    "execution_state": kernel["server"].last_activity["execution_state"],
+                    "connections": connections,
+                    "last_activity": last_activity,
+                    "execution_state": execution_state,
                 }
-                return result
+            )
+        return results
 
-        @router.post("/api/kernels/{kernel_id}/restart")
-        async def restart_kernel(
-            kernel_id,
-            user: User = Depends(auth.current_user(permissions={"kernels": ["write"]})),
-        ):
-            if kernel_id in kernels:
-                kernel = kernels[kernel_id]
-                await kernel["server"].restart()
-                result = {
-                    "id": kernel_id,
-                    "name": kernel["name"],
-                    "connections": kernel["server"].connections,
-                    "last_activity": kernel["server"].last_activity["date"],
-                    "execution_state": kernel["server"].last_activity["execution_state"],
-                }
-                return result
+    async def delete_session(
+        self,
+        session_id: str,
+        user: User,
+    ):
+        kernel_id = self.sessions[session_id].kernel.id
+        kernel_server = kernels[kernel_id]["server"]
+        await kernel_server.stop()
+        del kernels[kernel_id]
+        if kernel_id in self.kernel_id_to_connection_file:
+            del self.kernel_id_to_connection_file[kernel_id]
+        del self.sessions[session_id]
+        return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
-        @router.post("/api/kernels/{kernel_id}/execute")
-        async def execute_cell(
-            request: Request,
-            kernel_id,
-            user: User = Depends(auth.current_user(permissions={"kernels": ["write"]})),
-        ):
-            r = await request.json()
-            execution = Execution(**r)
-            if kernel_id in kernels:
-                ynotebook = yjs.YDocWebSocketHandler.websocket_server.get_room(
-                    execution.document_id
-                ).document
-                cell = ynotebook.get_cell(execution.cell_idx)
-                cell["outputs"] = []
-
-                kernel = kernels[kernel_id]
-                if not kernel["driver"]:
-                    kernel["driver"] = driver = KernelDriver(
-                        kernelspec_path=Path(find_kernelspec(kernel["name"])).as_posix(),
-                        write_connection_file=False,
-                        connection_file=kernel["server"].connection_file_path,
-                    )
-                    await driver.connect()
-                driver = kernel["driver"]
-
-                await driver.execute(cell)
-                ynotebook.set_cell(execution.cell_idx, cell)
-
-        @router.get("/api/kernels/{kernel_id}")
-        async def get_kernel(
-            kernel_id,
-            user: User = Depends(auth.current_user(permissions={"kernels": ["read"]})),
-        ):
-            if kernel_id in kernels:
-                kernel = kernels[kernel_id]
-                result = {
-                    "id": kernel_id,
-                    "name": kernel["name"],
-                    "connections": kernel["server"].connections,
-                    "last_activity": kernel["server"].last_activity["date"],
-                    "execution_state": kernel["server"].last_activity["execution_state"],
-                }
-                return result
+    async def rename_session(
+        self,
+        request: Request,
+        user: User,
+    ):
+        rename_session = await request.json()
+        session_id = rename_session.pop("id")
+        for key, value in rename_session.items():
+            setattr(self.sessions[session_id], key, value)
+        return self.sessions[session_id]
 
-        @router.delete("/api/kernels/{kernel_id}", status_code=204)
-        async def shutdown_kernel(
-            kernel_id,
-            user: User = Depends(auth.current_user(permissions={"kernels": ["write"]})),
-        ):
-            if kernel_id in kernels:
-                await kernels[kernel_id]["server"].stop()
-                del kernels[kernel_id]
-            for session_id in [k for k, v in sessions.items() if v.kernel.id == kernel_id]:
-                del sessions[session_id]
-            return Response(status_code=HTTPStatus.NO_CONTENT.value)
-
-        @router.websocket("/api/kernels/{kernel_id}/channels")
-        async def kernel_channels(
-            kernel_id,
-            session_id,
-            websocket_permissions=Depends(
-                auth.websocket_auth(permissions={"kernels": ["execute"]})
-            ),
-        ):
-            if websocket_permissions is None:
-                return
-            websocket, permissions = websocket_permissions
-            subprotocol = (
-                "v1.kernel.websocket.jupyter.org"
-                if "v1.kernel.websocket.jupyter.org" in websocket["subprotocols"]
-                else None
+    async def get_sessions(
+        self,
+        user: User,
+    ):
+        for session in self.sessions.values():
+            kernel_id = session.kernel.id
+            kernel_server = kernels[kernel_id]["server"]
+            session.kernel.last_activity = kernel_server.last_activity["date"]
+            session.kernel.execution_state = kernel_server.last_activity["execution_state"]
+        return list(self.sessions.values())
+
+    async def create_session(
+        self,
+        request: Request,
+        user: User,
+    ):
+        create_session = CreateSession(**(await request.json()))
+        kernel_id = create_session.kernel.id
+        kernel_name = create_session.kernel.name
+        if kernel_name is not None:
+            # launch a new ("internal") kernel
+            kernel_server = KernelServer(
+                kernelspec_path=Path(find_kernelspec(kernel_name)).as_posix(),
+                kernel_cwd=str(Path(create_session.path).parent),
             )
-            await websocket.accept(subprotocol=subprotocol)
-            accepted_websocket = AcceptedWebSocket(websocket, subprotocol)
-            if kernel_id in kernels:
-                kernel_server = kernels[kernel_id]["server"]
-                if kernel_server is None:
-                    # this is an external kernel
-                    # kernel is already launched, just start a kernel server
-                    kernel_server = KernelServer(
-                        connection_file=kernel_id,
-                        write_connection_file=False,
-                    )
-                    await kernel_server.start(launch_kernel=False)
-                    kernels[kernel_id]["server"] = kernel_server
-                await kernel_server.serve(accepted_websocket, session_id, permissions)
+            kernel_id = str(uuid.uuid4())
+            kernels[kernel_id] = {"name": kernel_name, "server": kernel_server, "driver": None}
+            await kernel_server.start()
+        elif kernel_id is not None:
+            # external kernel
+            kernel_name = kernels[kernel_id]["name"]
+            kernel_server = KernelServer(
+                connection_file=self.kernel_id_to_connection_file[kernel_id],
+                write_connection_file=False,
+            )
+            kernels[kernel_id]["server"] = kernel_server
+            await kernel_server.start(launch_kernel=False)
+        else:
+            return
+        session_id = str(uuid.uuid4())
+        session = Session(
+            id=session_id,
+            path=create_session.path,
+            name=create_session.name,
+            type=create_session.type,
+            kernel=Kernel(
+                id=kernel_id,
+                name=kernel_name,
+                connections=kernel_server.connections,
+                last_activity=kernel_server.last_activity["date"],
+                execution_state=kernel_server.last_activity["execution_state"],
+            ),
+            notebook=Notebook(
+                path=create_session.path,
+                name=create_session.name,
+            ),
+        )
+        self.sessions[session_id] = session
+        return session
 
-        self.include_router(router)
+    async def interrupt_kernel(
+        self,
+        kernel_id,
+        user: User,
+    ):
+        if kernel_id in kernels:
+            kernel = kernels[kernel_id]
+            kernel["server"].interrupt()
+            result = {
+                "id": kernel_id,
+                "name": kernel["name"],
+                "connections": kernel["server"].connections,
+                "last_activity": kernel["server"].last_activity["date"],
+                "execution_state": kernel["server"].last_activity["execution_state"],
+            }
+            return result
 
-        self.kernels = kernels
+    async def restart_kernel(
+        self,
+        kernel_id,
+        user: User,
+    ):
+        if kernel_id in kernels:
+            kernel = kernels[kernel_id]
+            await kernel["server"].restart()
+            result = {
+                "id": kernel_id,
+                "name": kernel["name"],
+                "connections": kernel["server"].connections,
+                "last_activity": kernel["server"].last_activity["date"],
+                "execution_state": kernel["server"].last_activity["execution_state"],
+            }
+            return result
+
+    async def execute_cell(
+        self,
+        request: Request,
+        kernel_id,
+        user: User,
+    ):
+        if self.yjs is None:
+            raise RuntimeError("Cannot execute without a Yjs plugin.")
+
+        r = await request.json()
+        execution = Execution(**r)
+        if kernel_id in kernels:
+            ynotebook = self.yjs.websocket_server.get_room(execution.document_id).document
+            cell = ynotebook.get_cell(execution.cell_idx)
+            cell["outputs"] = []
+
+            kernel = kernels[kernel_id]
+            if not kernel["driver"]:
+                kernel["driver"] = driver = KernelDriver(
+                    kernelspec_path=Path(find_kernelspec(kernel["name"])).as_posix(),
+                    write_connection_file=False,
+                    connection_file=kernel["server"].connection_file_path,
+                )
+                await driver.connect()
+            driver = kernel["driver"]
+
+            await driver.execute(cell)
+            ynotebook.set_cell(execution.cell_idx, cell)
+
+    async def get_kernel(
+        self,
+        kernel_id,
+        user: User,
+    ):
+        if kernel_id in kernels:
+            kernel = kernels[kernel_id]
+            result = {
+                "id": kernel_id,
+                "name": kernel["name"],
+                "connections": kernel["server"].connections,
+                "last_activity": kernel["server"].last_activity["date"],
+                "execution_state": kernel["server"].last_activity["execution_state"],
+            }
+            return result
+
+    async def shutdown_kernel(
+        self,
+        kernel_id,
+        user: User,
+    ):
+        if kernel_id in kernels:
+            await kernels[kernel_id]["server"].stop()
+            del kernels[kernel_id]
+        for session_id in [k for k, v in self.sessions.items() if v.kernel.id == kernel_id]:
+            del self.sessions[session_id]
+        return Response(status_code=HTTPStatus.NO_CONTENT.value)
+
+    async def kernel_channels(
+        self,
+        kernel_id,
+        session_id,
+        websocket_permissions,
+    ):
+        if websocket_permissions is None:
+            return
+        websocket, permissions = websocket_permissions
+        subprotocol = (
+            "v1.kernel.websocket.jupyter.org"
+            if "v1.kernel.websocket.jupyter.org" in websocket["subprotocols"]
+            else None
+        )
+        await websocket.accept(subprotocol=subprotocol)
+        accepted_websocket = AcceptedWebSocket(websocket, subprotocol)
+        if kernel_id in kernels:
+            kernel_server = kernels[kernel_id]["server"]
+            if kernel_server is None:
+                # this is an external kernel
+                # kernel is already launched, just start a kernel server
+                kernel_server = KernelServer(
+                    connection_file=kernel_id,
+                    write_connection_file=False,
+                )
+                await kernel_server.start(launch_kernel=False)
+                kernels[kernel_id]["server"] = kernel_server
+            await kernel_server.serve(accepted_websocket, session_id, permissions)
 
     async def watch_connection_files(self, path: Path) -> None:
         # first time scan, treat everything as added files
         initial_changes = {(Change.added, str(p)) for p in path.iterdir()}
         await self.process_connection_files(initial_changes)
         # then, on every change
         async for changes in awatch(path):
```

### Comparing `fps_kernels-0.1.3/fps_kernels/kernel_driver/connect.py` & `fps_kernels-0.1.4/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.3/fps_kernels/kernel_driver/driver.py` & `fps_kernels-0.1.4/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.3/fps_kernels/kernel_driver/kernelspec.py` & `fps_kernels-0.1.4/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.3/fps_kernels/kernel_driver/message.py` & `fps_kernels-0.1.4/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.3/fps_kernels/kernel_driver/paths.py` & `fps_kernels-0.1.4/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.3/fps_kernels/kernel_server/message.py` & `fps_kernels-0.1.4/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.3/fps_kernels/kernel_server/server.py` & `fps_kernels-0.1.4/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.3/.gitignore` & `fps_kernels-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.3/COPYING.md` & `fps_kernels-0.1.4/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.3/pyproject.toml` & `fps_kernels-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fps_kernels-0.1.3/PKG-INFO` & `fps_kernels-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fps_kernels
-Version: 0.1.3
+Version: 0.1.4
 Summary: An FPS plugin for the kernels API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
```


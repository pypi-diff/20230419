# Comparing `tmp/jsonrpc-py-3.0.0.tar.gz` & `tmp/jsonrpc-py-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonrpc-py-3.0.0.tar", last modified: Sun Apr 16 09:15:16 2023, max compression
+gzip compressed data, was "jsonrpc-py-3.0.1.tar", last modified: Wed Apr 19 09:30:06 2023, max compression
```

## Comparing `jsonrpc-py-3.0.0.tar` & `jsonrpc-py-3.0.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:15:16.005010 jsonrpc-py-3.0.0/
--rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2937 2023-04-16 09:15:16.005010 jsonrpc-py-3.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:15:15.998010 jsonrpc-py-3.0.0/jsonrpc/
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8885 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     4355 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     2219 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/errors.py
--rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5746 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/request.py
--rw-rw-rw-   0 root         (0) root         (0)     4055 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/response.py
--rw-rw-rw-   0 root         (0) root         (0)     1706 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/typedefs.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/jsonrpc/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:15:16.002010 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2937 2023-04-16 09:15:15.000000 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      658 2023-04-16 09:15:15.000000 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 09:15:15.000000 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 09:15:15.000000 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      134 2023-04-16 09:15:15.000000 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-04-16 09:15:15.000000 jsonrpc-py-3.0.0/jsonrpc_py.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      389 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/requirements-dev.txt
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-04-16 09:15:16.005010 jsonrpc-py-3.0.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)       61 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 09:15:16.005010 jsonrpc-py-3.0.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13845 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     3580 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_dispatcher.py
--rw-rw-rw-   0 root         (0) root         (0)     1917 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_errors.py
--rw-rw-rw-   0 root         (0) root         (0)     8121 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)     5721 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_response.py
--rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_serializer.py
--rw-rw-rw-   0 root         (0) root         (0)     2439 2023-04-16 09:15:04.000000 jsonrpc-py-3.0.0/tests/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:30:06.029232 jsonrpc-py-3.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1499 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-04-19 09:30:06.030149 jsonrpc-py-3.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1453 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:30:06.025565 jsonrpc-py-3.0.1/jsonrpc/
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9198 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4351 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     2219 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)       59 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5746 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/request.py
+-rw-rw-rw-   0 root         (0) root         (0)     4055 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1706 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/typedefs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1951 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/jsonrpc/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:30:06.027398 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-04-19 09:30:05.000000 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      658 2023-04-19 09:30:05.000000 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:30:05.000000 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 09:30:05.000000 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      134 2023-04-19 09:30:05.000000 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-19 09:30:05.000000 jsonrpc-py-3.0.1/jsonrpc_py.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      389 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      127 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/requirements-dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-04-19 09:30:06.030149 jsonrpc-py-3.0.1/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)       61 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 09:30:06.029232 jsonrpc-py-3.0.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13845 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     3580 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_dispatcher.py
+-rw-rw-rw-   0 root         (0) root         (0)     1917 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     8121 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     5721 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_response.py
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_serializer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2023-04-19 09:29:54.000000 jsonrpc-py-3.0.1/tests/test_utilities.py
```

### Comparing `jsonrpc-py-3.0.0/LICENSE` & `jsonrpc-py-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/PKG-INFO` & `jsonrpc-py-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.0
+Version: 3.0.1
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Home-page: https://docs.jsonrpc.ru
 Author: Andrew Malchuk
 Author-email: andrew.malchuk@yandex.ru
 Maintainer: JSON-RPC Development Group
 Maintainer-email: dev@jsonrpc.ru
 License: BSD-3-Clause
```

### Comparing `jsonrpc-py-3.0.0/README.md` & `jsonrpc-py-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/jsonrpc/asgi.py` & `jsonrpc-py-3.0.1/jsonrpc/asgi.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from asyncio import CancelledError, Task, create_task, gather, wait_for
 from collections import UserDict
-from collections.abc import MutableSequence
+from collections.abc import Generator, MutableSequence
 from http import HTTPMethod, HTTPStatus
-from io import BytesIO
-from typing import Any, ClassVar, Final, Self, TypeAlias
+from io import DEFAULT_BUFFER_SIZE, BytesIO
+from typing import Any, ClassVar, Final, TypeAlias
 
 from .dispatcher import AsyncDispatcher
 from .errors import Error
 from .request import BatchRequest, Request
 from .response import BatchResponse, Response
 from .serializer import JSONSerializer
 from .typedefs import ASGIReceiveCallable, ASGISendCallable, HTTPConnectionScope, Scope
@@ -29,35 +29,38 @@
     __slots__: tuple[str, ...] = ("status",)
 
     def __init__(self, *, status: HTTPStatus) -> None:
         self.status: Final[HTTPStatus] = status
 
 
 class HTTPHandler:
-    __slots__: tuple[str, ...] = ("scope", "receive", "send", "app", "background_tasks")
+    """
+    Main HTTP endpoint.
+    """
+
+    __slots__: tuple[str, ...] = ("scope", "receive", "send", "app")
+
+    #: ---
+    #: Avoid a "fire-and-forget" background tasks disappearing mid-execution:
+    background_tasks: Final[set[AnyTask]] = set()
 
     def __init__(
         self,
-        *,
         scope: HTTPConnectionScope,
         receive: ASGIReceiveCallable,
         send: ASGISendCallable,
         app: type["ASGIHandler"],
     ) -> None:
         self.scope: Final[HTTPConnectionScope] = scope
         self.receive: Final[ASGIReceiveCallable] = receive
         self.send: Final[ASGISendCallable] = send
         self.app: type[ASGIHandler] = app
-        self.background_tasks: set[AnyTask] = set()
-
-    def __enter__(self) -> Self:
-        return self
 
-    def __exit__(self, *args: Any) -> None:
-        return None
+    def __await__(self) -> Generator[Any, None, None]:
+        return self.dispatch().__await__()
 
     async def dispatch(self) -> None:
         try:
             #: ---
             #: Might be "405 Method Not Allowed" or "415 Unsupported Media Type".
             self.negotiate_content()
 
@@ -102,27 +105,40 @@
                         if not kwargs.get("more_body", False):
                             break
                     case {"type": "http.disconnect"}:
                         raise RequestAborted("Client was disconnected too early.")
 
             return raw_buffer.getvalue()
 
-    async def send_response(self, *, status: HTTPStatus = HTTPStatus.OK, payload: bytes = b"") -> None:
+    async def send_response(
+        self,
+        *,
+        status: HTTPStatus = HTTPStatus.OK,
+        payload: bytes = b"",
+        buffer_size: int = DEFAULT_BUFFER_SIZE,
+    ) -> None:
         headers: list[tuple[bytes, bytes]] = [
             (b"content-type", self.app.content_type.encode("ascii")),
         ]
         if status == HTTPStatus.METHOD_NOT_ALLOWED:
             headers.append((b"allow", HTTPMethod.POST.encode("ascii")))
             headers.sort()
         #: ---
-        #: Start sending a response message.
+        #: Initial response message:
         await self.send({"type": "http.response.start", "status": status, "headers": headers})
         #: ---
-        #: Finish a response message with payload.
-        await self.send({"type": "http.response.body", "body": payload, "more_body": False})
+        #: Yield chunks of response:
+        with BytesIO(payload) as raw_buffer:
+            try:
+                while chunk := raw_buffer.read(buffer_size):
+                    await self.send({"type": "http.response.body", "body": chunk, "more_body": True})
+            finally:
+                #: ---
+                #: Final closing message:
+                await self.send({"type": "http.response.body", "body": b"", "more_body": False})
 
     async def parse_payload(self, payload: bytes) -> bytes:
         def write_error(error: Error) -> bytes:
             response: Response = Response(error=error, response_id=None)
             return self.app.serializer.serialize(response.json)
 
         try:
@@ -215,16 +231,10 @@
 
     def __repr__(self) -> str:
         return f"{self.__class__.__qualname__}({self.data!r})"
 
     async def __call__(self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable) -> None:
         match scope:
             case {"type": "http", **kwargs}:  # noqa: F841
-                with HTTPHandler(
-                    scope=scope,  # type: ignore[arg-type]
-                    receive=receive,
-                    send=send,
-                    app=self.__class__,
-                ) as handler:
-                    await handler.dispatch()
+                return await HTTPHandler(scope, receive, send, self.__class__)  # type: ignore[arg-type]
             case _:
                 raise ValueError("Only ASGI/HTTP connections are allowed.")
```

### Comparing `jsonrpc-py-3.0.0/jsonrpc/dispatcher.py` & `jsonrpc-py-3.0.1/jsonrpc/dispatcher.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections import UserDict
 from collections.abc import Callable
 from functools import partial
 from inspect import BoundArguments, isfunction, signature
 from typing import Any, Final, TypeAlias, TypeVar, overload
 
 from .errors import Error, ErrorEnum
-from .utilities import wrap_coroutine
+from .utilities import ensure_async
 
 __all__: Final[tuple[str, ...]] = ("AsyncDispatcher",)
 
 AnyCallable: TypeAlias = Callable[..., Any]
 Func = TypeVar("Func", bound=AnyCallable)
 
 
@@ -94,12 +94,12 @@
 
         try:
             params: BoundArguments = signature(user_function).bind(*args, **kwargs)
         except TypeError as exc:
             raise Error(code=ErrorEnum.INVALID_PARAMETERS, message=f"Invalid parameters: {exc!s}") from exc
 
         try:
-            return await wrap_coroutine(user_function, *params.args, **params.kwargs)
+            return await ensure_async(user_function, *params.args, **params.kwargs)
         except (TimeoutError, CancelledError, Error):
             raise
         except Exception as exc:
             raise Error(code=ErrorEnum.INTERNAL_ERROR, message=f"Unexpected internal error: {exc!s}") from exc
```

### Comparing `jsonrpc-py-3.0.0/jsonrpc/errors.py` & `jsonrpc-py-3.0.1/jsonrpc/errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/jsonrpc/request.py` & `jsonrpc-py-3.0.1/jsonrpc/request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/jsonrpc/response.py` & `jsonrpc-py-3.0.1/jsonrpc/response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/jsonrpc/serializer.py` & `jsonrpc-py-3.0.1/jsonrpc/serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/jsonrpc/typedefs.py` & `jsonrpc-py-3.0.1/jsonrpc/typedefs.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/jsonrpc/utilities.py` & `jsonrpc-py-3.0.1/jsonrpc/utilities.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,34 @@
 from collections.abc import Callable, Iterable, MutableMapping
 from contextvars import Context, copy_context
 from functools import partial
 from inspect import iscoroutinefunction
 from typing import Any, Final, Literal, ParamSpec, TypeGuard, final
 
 __all__: Final[tuple[str, ...]] = (
+    "ensure_async",
     "is_iterable",
     "make_hashable",
     "Undefined",
     "UndefinedType",
-    "wrap_coroutine",
 )
 
 P = ParamSpec("P")
 
 
+def ensure_async(user_function: Callable[P, Any], /, *args: P.args, **kwargs: P.kwargs) -> Future[Any]:
+    loop: AbstractEventLoop = get_running_loop()
+    context: Context = copy_context()
+
+    if iscoroutinefunction(callback := partial(user_function, *args, **kwargs)):
+        return loop.create_task(callback(), context=context)
+    else:
+        return loop.run_in_executor(None, context.run, callback)
+
+
 def is_iterable(obj: Any, /) -> TypeGuard[Iterable[Any]]:
     try:
         iter(obj)
     except TypeError:
         return False
     else:
         return True
@@ -39,24 +49,14 @@
         #: ---
         #: Non-hashable, non-iterable:
         raise
 
     return obj
 
 
-def wrap_coroutine(user_function: Callable[P, Any], /, *args: P.args, **kwargs: P.kwargs) -> Future[Any]:
-    loop: AbstractEventLoop = get_running_loop()
-    context: Context = copy_context()
-
-    if iscoroutinefunction(callback := partial(user_function, *args, **kwargs)):
-        return loop.create_task(callback(), context=context)
-    else:
-        return loop.run_in_executor(None, context.run, callback)
-
-
 @final
 class UndefinedType:
     __slots__: tuple[str, ...] = ()
 
     def __repr__(self) -> Literal["Undefined"]:
         return "Undefined"
```

### Comparing `jsonrpc-py-3.0.0/jsonrpc_py.egg-info/PKG-INFO` & `jsonrpc-py-3.0.1/jsonrpc_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonrpc-py
-Version: 3.0.0
+Version: 3.0.1
 Summary: Pure zero-dependency JSON-RPC 2.0 implementation
 Home-page: https://docs.jsonrpc.ru
 Author: Andrew Malchuk
 Author-email: andrew.malchuk@yandex.ru
 Maintainer: JSON-RPC Development Group
 Maintainer-email: dev@jsonrpc.ru
 License: BSD-3-Clause
```

### Comparing `jsonrpc-py-3.0.0/jsonrpc_py.egg-info/SOURCES.txt` & `jsonrpc-py-3.0.1/jsonrpc_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/setup.cfg` & `jsonrpc-py-3.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/tests/test_asgi.py` & `jsonrpc-py-3.0.1/tests/test_asgi.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/tests/test_dispatcher.py` & `jsonrpc-py-3.0.1/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/tests/test_errors.py` & `jsonrpc-py-3.0.1/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/tests/test_request.py` & `jsonrpc-py-3.0.1/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/tests/test_response.py` & `jsonrpc-py-3.0.1/tests/test_response.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/tests/test_serializer.py` & `jsonrpc-py-3.0.1/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `jsonrpc-py-3.0.0/tests/test_utilities.py` & `jsonrpc-py-3.0.1/tests/test_utilities.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from asyncio import Future
 from typing import Any, Literal
 from unittest import IsolatedAsyncioTestCase, TestCase
 from unittest.mock import AsyncMock, MagicMock, sentinel
 
-from jsonrpc.utilities import Undefined, UndefinedType, make_hashable, wrap_coroutine
+from jsonrpc.utilities import Undefined, UndefinedType, ensure_async, make_hashable
 
 
 class TestHashable(TestCase):
     def test_equality(self) -> None:
         tests: tuple[tuple[Any, Any], ...] = (
             ([], ()),
             (["a", 1], ("a", 1)),
@@ -51,17 +50,16 @@
         self.assertNotEqual(Undefined, None)
 
     def test_is_truth(self) -> None:
         self.assertFalse(Undefined)
 
 
 class TestUtilities(IsolatedAsyncioTestCase):
-    async def test_wrap_coroutine(self) -> None:
+    async def test_ensure_async(self) -> None:
         for mock in (
             MagicMock(return_value=sentinel.sync_def),
             AsyncMock(return_value=sentinel.async_def),
         ):
             with self.subTest(mock=mock):
-                future: Future[Any] = wrap_coroutine(mock, 1, 2, 3, key="value")
-                self.assertIsInstance(future, Future)
-                self.assertIs(await future, mock.return_value)
+                result: Any = await ensure_async(mock, 1, 2, 3, key="value")
+                self.assertIs(result, mock.return_value)
                 mock.assert_called_once_with(1, 2, 3, key="value")
```


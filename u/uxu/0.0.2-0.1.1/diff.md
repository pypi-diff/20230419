# Comparing `tmp/uxu-0.0.2.tar.gz` & `tmp/uxu-0.1.1.tar.gz`

## Comparing `uxu-0.0.2.tar` & `uxu-0.1.1.tar`

### file list

```diff
@@ -1,76 +1,42 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 uxu-0.0.2/.env
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 uxu-0.0.2/pyrightconfig.json
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/0a1237d725462fae/352387855ee8c379
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/0a1237d725462fae/cd6bd1dcfebeffe9
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/1e4bdf158bd9b9e5/394341b7182cd227
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/1e4bdf158bd9b9e5/7d0fdd8cd1d85fd3
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/476fb78351979deb/1dd6f7b457ad880d
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/476fb78351979deb/c32bb284c4a9bfae
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/77d3df0ea028b111/352387855ee8c379
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/77d3df0ea028b111/5ac597c988feda25
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/77d3df0ea028b111/7089cef4b92d73cc
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/77d3df0ea028b111/cd6bd1dcfebeffe9
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/a1b87770545a8882/1dd6f7b457ad880d
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/examples/a1b87770545a8882/c32bb284c4a9bfae
--rw-r--r--   0        0        0    20988 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/unicode_data/13.0.0/charmap.json.gz
--rw-r--r--   0        0        0    21505 2020-02-02 00:00:00.000000 uxu-0.0.2/.hypothesis/unicode_data/14.0.0/charmap.json.gz
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 uxu-0.0.2/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 uxu-0.0.2/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 uxu-0.0.2/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 uxu-0.0.2/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 uxu-0.0.2/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 uxu-0.0.2/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 uxu-0.0.2/.vscode/launch.json
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 uxu-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 uxu-0.0.2/tests/test_listdiff.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 uxu-0.0.2/tests/test_patch.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/__about__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/__init__.py
--rw-r--r--   0        0        0     5205 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/element.py
--rw-r--r--   0        0        0    11760 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/fiber.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/html.py
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/listdiff.py
--rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/manager.py
--rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/patch.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/persistence.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/proxy_reactor.py
--rw-r--r--   0        0        0     6046 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rendering.py
--rw-r--r--   0        0        0     9102 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/serve.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/textnode.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/util.py
--rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/vdom.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/lsp/README.md
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/lsp/__init__.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/lsp/server.py
--rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/lsp/types.py
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rpc/__init__.py
--rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rpc/io_transport.py
--rw-r--r--   0        0        0    18290 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rpc/jsonrpc.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rpc/starlette_ws_transport.py
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rpc/transport.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 uxu-0.0.2/uxu/rpc/websocket_transport.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 uxu-0.0.2/web/.gitignore
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 uxu-0.0.2/web/build.mjs
--rw-r--r--   0        0        0    14308 2020-02-02 00:00:00.000000 uxu-0.0.2/web/package-lock.json
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 uxu-0.0.2/web/package.json
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 uxu-0.0.2/web/server.mjs
--rw-r--r--   0        0        0     2358 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/.package-lock.json
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/.bin/esbuild -> ../esbuild/bin/esbuild
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/@esbuild/darwin-arm64/README.md
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/@esbuild/darwin-arm64/package.json
--rwxr-xr-x   0        0        0  8858802 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/@esbuild/darwin-arm64/bin/esbuild
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/LICENSE.md
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/README.md
--rw-r--r--   0        0        0    10703 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/install.js
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/package.json
-hrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/bin/esbuild
--rw-r--r--   0        0        0    18934 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/lib/main.d.ts
--rw-r--r--   0        0        0    86013 2020-02-02 00:00:00.000000 uxu-0.0.2/web/node_modules/esbuild/lib/main.js
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 uxu-0.0.2/web/src/app.ts
--rw-r--r--   0        0        0    13701 2020-02-02 00:00:00.000000 uxu-0.0.2/web/src/reactor.ts
--rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 uxu-0.0.2/web/src/rpc.ts
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 uxu-0.0.2/.gitignore
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 uxu-0.0.2/LICENSE.txt
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 uxu-0.0.2/README.md
--rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 uxu-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 uxu-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 uxu-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 uxu-0.1.1/tests/test_listdiff.py
+-rw-r--r--   0        0        0     3572 2020-02-02 00:00:00.000000 uxu-0.1.1/tests/test_patch.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/__about__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/__init__.py
+-rw-r--r--   0        0        0     5201 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/element.py
+-rw-r--r--   0        0        0    11760 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/fiber.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/html.py
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/listdiff.py
+-rw-r--r--   0        0        0     5153 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/manager.py
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/patch.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/persistence.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/proxy_reactor.py
+-rw-r--r--   0        0        0     6042 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/rendering.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/serve.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/session.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/textnode.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/util.py
+-rw-r--r--   0        0        0     5095 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/vdom.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/lsp/README.md
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/lsp/__init__.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/lsp/server.py
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/lsp/types.py
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/rpc/__init__.py
+-rw-r--r--   0        0        0     2711 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/rpc/io_transport.py
+-rw-r--r--   0        0        0    18781 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/rpc/jsonrpc.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/rpc/starlette_ws_transport.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/rpc/transport.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 uxu-0.1.1/uxu/rpc/websocket_transport.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 uxu-0.1.1/web/.gitignore
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 uxu-0.1.1/web/build.mjs
+-rw-r--r--   0        0        0    14308 2020-02-02 00:00:00.000000 uxu-0.1.1/web/package-lock.json
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 uxu-0.1.1/web/package.json
+-rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 uxu-0.1.1/web/server.mjs
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 uxu-0.1.1/web/src/app.ts
+-rw-r--r--   0        0        0    14337 2020-02-02 00:00:00.000000 uxu-0.1.1/web/src/reactor.ts
+-rw-r--r--   0        0        0     5434 2020-02-02 00:00:00.000000 uxu-0.1.1/web/src/rpc.ts
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 uxu-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 uxu-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 uxu-0.1.1/README.md
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 uxu-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 uxu-0.1.1/PKG-INFO
```

### Comparing `uxu-0.0.2/tests/test_listdiff.py` & `uxu-0.1.1/tests/test_listdiff.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/tests/test_patch.py` & `uxu-0.1.1/tests/test_patch.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,16 @@
     div("hello", "world"),
     div("world", "hello"),
     div("hello"),
     div("hello", "hello"),
     div(),
     div(div("cheese", key="x"), div("world", key="y")),
     div(div("cheese", key="x"), div("world", key="x")),
-    h("span", {}, key="x"),
-    h("div", {}, key="x"),
+    h("span", key="x"),
+    h("div", key="x"),
     div(x="y"),
     div(x="z"),
     div(x="y", y="x"),
 ]
 
 
 def test_examples():
@@ -95,15 +95,15 @@
     assert p.reorder.l1_len == p.reorder.l2_len
 
 
 @pytest.mark.asyncio
 async def test_button():
     def C(x: str):
         y = useState("1")
-        return h("button", {"onclick": lambda _: y.set("2")}, [x, y.current])
+        return h("button", [x, y.current], onclick = lambda _: y.set("2"))
 
     with Manager() as m:
         m.initialize(h(C, "x"))
         r1 = m.render()
         assert isinstance(r1, RootRendering)
         assert len(r1.children) == 1
         f = r1.children[0]
```

### Comparing `uxu-0.0.2/uxu/element.py` & `uxu-0.1.1/uxu/element.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     hydrate_lists,
     patch,
     reconcile_lists,
     vdom_context,
 )
 from .rendering import Rendering, RenderedElement
 
-logger = logging.getLogger("reactor")
+logger = logging.getLogger("uxu")
 
 
 @dataclass
 class ElementSpec(NormSpec):
     tag: str
     attrs: dict
     children: list[NormSpec]
```

### Comparing `uxu-0.0.2/uxu/fiber.py` & `uxu-0.1.1/uxu/fiber.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/uxu/listdiff.py` & `uxu-0.1.1/uxu/listdiff.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/uxu/manager.py` & `uxu-0.1.1/uxu/manager.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/uxu/patch.py` & `uxu-0.1.1/uxu/patch.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/uxu/persistence.py` & `uxu-0.1.1/uxu/persistence.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/uxu/proxy_reactor.py` & `uxu-0.1.1/uxu/proxy_reactor.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/uxu/rendering.py` & `uxu-0.1.1/uxu/rendering.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         assert isinstance(elt, dom_tag)
         return elt
 
 
 @dataclass
 class RenderedFragment(Rendering):
     id: Any
-    children: list["Rendering"]
+    children: list[Rendering]
     key: Any = field(default=None)
     kind: ClassVar[str] = "fragment"
 
     def static(self):
         return [c.static() for c in self.children]
 
 
@@ -186,15 +186,15 @@
     id: Any
     name: str
     props: Any
     kind: ClassVar[str] = "widget"
 
 
 # [todo] put on Rendering methods
-def iter_event_handlers(x: "Rendering"):
+def iter_event_handlers(x: Rendering):
     if isinstance(x, RenderedElement):
         for name, v in x.attrs.items():
             if isinstance(v, EventHandler):
                 yield name, v
     children = getattr(x, "children", [])
     for child in children:
         yield from iter_event_handlers(child)
```

### Comparing `uxu-0.0.2/uxu/serve.py` & `uxu-0.1.1/uxu/serve.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,63 @@
 from uuid import UUID, uuid4
 import logging
 
 from pydantic import BaseModel, BaseSettings, Field, SecretStr
 import dominate
 import dominate.tags as t
 from jose import ExpiredSignatureError, JWTError, jwt
-
+import tempfile
 from starlette.responses import HTMLResponse
 from starlette.requests import Request
 from starlette.routing import Route, Mount, WebSocketRoute
 from starlette.applications import Starlette
 from starlette.staticfiles import StaticFiles
 from starlette.websockets import WebSocket
+from uxu.fiber import useState
 
 from uxu.manager import EventArgs, Manager, render_static
 from uxu.persistence import PersistDict
 from uxu.rpc import (
     StarletteWebsocketTransport,
     RpcServer,
     InitializationMode,
     Transport,
 )
 from uxu.__about__ import __version__
 from uxu.rpc.jsonrpc import invalid_params, rpc_method
 from uxu.html import h
 from uxu.rendering import RootRendering
+from uxu.session import UxuSession
+from uxu.vdom import Html
 
 # https://fastapi.tiangolo.com/advanced/websockets/?h=websocket
 
 logger = logging.getLogger("uxu")
 
 
+def Counter() -> Html:
+    x = useState(0)
+    return h(
+        "div",
+        [
+            h("button", ["+"], click=lambda _: x.modify(lambda x: x + 1)),
+            str(x.current),
+            h("button", ["-"], click=lambda _: x.modify(lambda x: x - 1)),
+        ],
+    )
+
+
 def HelloWorld(text: str):
     """Just a simple component to test things."""
     return h(
-        "main",
-        {},
+        "div",
         [
-            h("h1", {}, "Hello World"),
-            h("p", {}, ["The content was: ", text]),
+            h("h1", "Hello World"),
+            h("p", ["The content was: ", text]),
+            h(Counter),
         ],
     )
 
 
 def component_of_name(name: str):
     return HelloWorld
 
@@ -58,34 +73,42 @@
     id: str  # session id
     component_name: str
     path: str
     rendering: RootRendering
     params: dict[str, str] = field(default_factory=dict)
 
 
+# https://stackoverflow.com/questions/66093397/how-to-disable-starlette-static-files-caching
+class MyStatics(StaticFiles):
+    def is_not_modified(self, response_headers, request_headers) -> bool:
+        # your own cache rules goes here...
+        return False
+
+
 class UxuApplication:
     """
     I'm not completely sure how this should work yet, but the idea is that
     UxuApplication is a valid ASGI app that you can dump into Starlette or FastAPI or whatever.
 
     For now, I'm just doing dependency injection but I want to do this properly.
+    [todo] allow turning off auth ticketing.
 
     """
 
     def __init__(self):
         self.cfg = Settings()  # type: ignore
         self.persistence = PersistDict(
             self.cfg.persistent_dict_path, T=UxuSessionParams
         )
         self.webapp = Starlette(
             debug=True,
             routes=[
                 Mount(
                     "/static",
-                    app=StaticFiles(packages=[("uxu", "static")]),
+                    app=MyStatics(packages=[("uxu", "static")]),
                     name="static",
                 ),
                 # https://www.starlette.io/routing#websocket-routing
                 WebSocketRoute("/ws", endpoint=self.handle_websocket),
                 Route("/{name:str}", self.handle),
             ],
         )
@@ -150,15 +173,15 @@
 
         content = document.render()
         return HTMLResponse(content=content)
 
     async def handle_websocket(self, websocket: WebSocket):
         await websocket.accept()
         transport = StarletteWebsocketTransport(websocket)
-        with UxuSession(
+        with UxuWebSession(
             transport, self.persistence, socket_url=str(websocket.url)
         ) as server:
             await server.serve_forever()
         await websocket.close()
 
 
 class TicketClaims(BaseModel):
@@ -169,17 +192,21 @@
     iss: str
     sub: Optional[UUID]
 
 
 class Settings(BaseSettings):
     jwt_expires: timedelta = Field(default=timedelta(hours=2))
     jwt_algorithm: str = Field(default="HS256")
-    jwt_secret: SecretStr
+    jwt_secret: SecretStr = Field(
+        default_factory=lambda: SecretStr("watch out this is the default string!")
+    )
 
-    persistent_dict_path: Path = Field(default=Path("tmp/uxu_server.sqlite"))
+    persistent_dict_path: Path = Field(
+        default_factory=lambda: Path(tempfile.gettempdir()) / "uxu_server.sqlite"
+    )
 
     class Config:
         env_file = ".env"
         env_file_encoding = "utf-8"
 
 
 class PeerInfo(BaseModel):
@@ -194,27 +221,26 @@
     # [todo] some kind of DOM checksum
 
 
 class UxuInitResponse(BaseModel):
     serverInfo: PeerInfo
 
 
-class UxuSession(RpcServer):
+class UxuWebSession(UxuSession):
     """Handles a websocket session."""
 
     def __init__(
         self,
         transport: Transport,
         persistence: PersistDict[UxuSessionParams],
         socket_url: str,
     ):
-        super().__init__(transport, init_mode=InitializationMode.ExpectInit)
+        super().__init__(transport=transport, spec=None)
         self.persistence = persistence
         self.socket_url = socket_url
-        self.manager = Manager(is_static=False)
 
     @rpc_method("initialize")
     async def on_initialize(self, params: UxuInitParams):
         cfg = Settings()  # type: ignore
         if not isinstance(params, UxuInitParams):
             raise invalid_params()
         claims = jwt.decode(
@@ -238,53 +264,14 @@
         self.manager.hydrate(session_params.rendering, spec)
         self.patch_task = asyncio.create_task(self.patcher_loop())
 
         return UxuInitResponse(
             serverInfo=PeerInfo(name="uxu-server", version=__version__)
         )
 
-    @rpc_method("initialized")
-    def on_initialized(self, params):
-        logger.debug("client successfully initialized")
-        return
-
-    @rpc_method("render")
-    def on_render(self, params):
-        """Request to render."""
-        return self.manager.render()
-
-    @rpc_method("event")
-    def handle_event(self, params: EventArgs):
-        return self.manager.handle_event(params)
-
-    async def patcher_loop(self):
-        while True:
-            try:
-                patches = await self.manager.wait_patches()
-                if len(patches) > 0:
-                    result = await self.request("patch", patches)
-                    # [todo] send encoded patches
-                    logger.debug(f"patcher_loop patched: {result}")
-            except asyncio.CancelledError:
-                logger.debug("patcher_loop: cancelled")
-                break
-            except Exception as e:
-                # [todo] this is for debugging only
-                logger.exception("patcher_loop threw an exception")
-                break
-        logger.debug("patcher_loop: done")
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        if hasattr(self, "patch_task"):
-            self.patch_task.cancel()
-        self.manager.dispose()
-
 
 app = UxuApplication()
 
 from rich.logging import RichHandler
 
 FORMAT = "%(message)s"
 logging.basicConfig(
```

### Comparing `uxu-0.0.2/uxu/textnode.py` & `uxu-0.1.1/uxu/textnode.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/uxu/vdom.py` & `uxu-0.1.1/uxu/vdom.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/uxu/lsp/server.py` & `uxu-0.1.1/uxu/lsp/server.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,8 +20,8 @@
         return InitializeResult(
             serverInfo=PeerInfo(name=self.name, version=None),
             capabilities=self.capabilities,
         )
 
     @rpc_method("initialized")
     async def on_client_initialized(self, params):
-        logger.info("Client initialized")
+        logger.info("client initialized")
```

### Comparing `uxu-0.0.2/uxu/lsp/types.py` & `uxu-0.1.1/uxu/lsp/types.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/uxu/rpc/io_transport.py` & `uxu-0.1.1/uxu/rpc/io_transport.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/uxu/rpc/jsonrpc.py` & `uxu-0.1.1/uxu/rpc/jsonrpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from miniscutil.ofdict import MyJsonEncoder, ofdict
 import json
 from .transport import Transport, TransportClosedError, TransportClosedOK
 
 from websockets.exceptions import ConnectionClosedOK, ConnectionClosedError
 
-logger = logging.getLogger("jsonrpc")
+logger = logging.getLogger(__name__)
 
 
 class ErrorCode(Enum):
     ### JSON-RPC codes
 
     parse_error = -32700
     """ It doesn't parse as JSON """
@@ -75,14 +75,20 @@
     @property
     def is_notification(self):
         return self.id is None
 
     def to_bytes(self):
         return encoder.encode(self).encode()
 
+    def __str__(self):
+        if self.id is None:
+            return f"notify {self.method}"
+        else:
+            return f"request {self.method}:{self.id}"
+
 
 @dataclass
 class ResponseError(Exception):
     code: ErrorCode
     message: str
     data: Optional[Any] = field(default=None)
 
@@ -255,15 +261,15 @@
     [todo] instead of needing to explicitly register methods, make a decorator.
     """
 
     dispatcher: Dispatcher
     status: RpcServerStatus
     transport: Transport
     init_mode: InitializationMode
-    name : str
+    name: str
     request_counter: int
     """ Unique id for each request I make to the peer. """
     my_requests: Dict[RequestId, Future[Any]]
     """ Requests that I have made to my peer. """
     their_requests: Dict[RequestId, Task]
     """ Requests that my peer has made to me. """
     notification_tasks: set[asyncio.Task]
@@ -272,14 +278,18 @@
     def __init__(
         self,
         transport: Transport,
         dispatcher=None,
         name=None,
         init_mode: InitializationMode = InitializationMode.NoInit,
     ):
+        if not isinstance(transport, Transport):
+            raise TypeError(
+                f"transport must be an instance of uxu.rpc.Transport, not {type(transport)}"
+            )
         global server_count
         server_count += 1
         if name is None:
             self.name = f"<{type(self).__name__} {server_count}>"
         else:
             assert isinstance(name, str)
             self.name = name
@@ -386,14 +396,17 @@
                         error=ResponseError(message=str(e), code=ErrorCode.parse_error)
                     )
                     await self.send(response)
                     continue
                 except ExitNotification as e:
                     logger.info(f"{self.name} received exit notification, terminating")
                     return
+                except KeyboardInterrupt as e:
+                    logger.exception(f"recieved kb interrupt, terminating")
+                    return
         finally:
             logger.info(f"exiting serve_forever loop")
             (_, e, _) = sys.exc_info()  # sys.exception() is 3.11 only
             if e is None:
                 e = ConnectionError(f"{self} shutdown")
             for fut in self.my_requests.values():
                 fut.set_exception(e)
@@ -426,15 +439,15 @@
                     logger.warning("exit notification received before shutdown request")
                 # https://microsoft.github.io/language-server-protocol/specifications/lsp/3.17/specification/#exit
                 raise ExitNotification()
             if req.method == "shutdown":
                 self._shutdown()
             task = asyncio.create_task(
                 self._on_request(req),
-                name=f"{self.name} handle {req.method} {req.id or ''} ",
+                name=f"{self.name} handle {req}",
             )
             id = req.id
             if id is not None:
                 self.their_requests[id] = task
                 task.add_done_callback(lambda _: self.their_requests.pop(id))
             else:
                 self.notification_tasks.add(task)
@@ -452,15 +465,15 @@
                             code=ErrorCode.request_cancelled, message=str(e)
                         ),
                     )
                 )
         except ResponseError as e:
             await self.send(Response(id=req.id, error=e))
         except Exception as e:
-            logger.exception(f"{self} {req.id} unhandled exception")
+            logger.exception(f"{self} {req} unhandled exception. data:\n{req.params}")
             await self.send(
                 Response(
                     id=req.id,
                     error=ResponseError(code=ErrorCode.server_error, message=str(e)),
                 )
             )
         else:
```

### Comparing `uxu-0.0.2/uxu/rpc/starlette_ws_transport.py` & `uxu-0.1.1/uxu/rpc/starlette_ws_transport.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/uxu/rpc/transport.py` & `uxu-0.1.1/uxu/rpc/transport.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from abc import ABC, abstractmethod
 from typing import Awaitable, Protocol
 
 """
 Abstract definition of Transport for RPC.
 
 [todo] use tinyrpc?
 """
@@ -27,22 +28,24 @@
     pass
 
 
 class TransportError(Exception):
     """Transport recieved an invalid or corrupted message."""
 
 
-class Transport(Protocol):
+class Transport(ABC):
     """Abstract datagram transport. Data can be sent and recieved in finite-length bytestring messages."""
 
+    @abstractmethod
     def recv(self) -> Awaitable[bytes]:
         """Wait to recieve the a message.
 
         Raises:
           TransportClosedOK: if the transport is closed properly.
           TransportClosedError: if the transport is closed with an error.
           TransportError: if the transport recieved an invalid or corrupted message or some other error where the connection is not closed.
         """
         ...
 
+    @abstractmethod
     def send(self, data: bytes) -> Awaitable[None]:
         ...
```

### Comparing `uxu-0.0.2/uxu/rpc/websocket_transport.py` & `uxu-0.1.1/uxu/rpc/websocket_transport.py`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/web/build.mjs` & `uxu-0.1.1/web/build.mjs`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/web/package-lock.json` & `uxu-0.1.1/web/package-lock.json`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/web/server.mjs` & `uxu-0.1.1/web/server.mjs`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/web/node_modules/esbuild/LICENSE.md` & `uxu-0.1.1/LICENSE.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,9 @@
 MIT License
 
-Copyright (c) 2020 Evan Wallace
+Copyright (c) 2023-present E.W.Ayers <contact@edayers.com>
 
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `uxu-0.0.2/web/src/reactor.ts` & `uxu-0.1.1/web/src/reactor.ts`

 * *Files 4% similar despite different names*

```diff
@@ -48,20 +48,34 @@
     create(props: P): Element
     reconcile(previous_node: Element, previous_props: P, new_props: P): void
     dispose(node: Element): void
 }
 
 type Rendering = RenderedText | RenderedElement | RenderedFragment | RenderedWidget
 
+interface Reorder {
+    l1_len: number
+    l2_len: number
+    remove_these: { [key: string]: null | string }
+    then_insert_these: { [key: string]: [0, string] | [1, Rendering] }
+}
+
 interface ModifyChildrenPatch {
     kind: 'modify-children'
     element_id: string;
-    children_length_start: number;
-    remove_these: Map<number, null | string>
-    then_insert_these: Map<number, [0, string] | [1, Rendering]>
+    reorder: Reorder;
+}
+
+function mapOfObject<T>(obj: { [key: string]: T }): Map<number, T> {
+    const map = new Map()
+    for (const key of Object.keys(obj)) {
+        const value = obj[key]
+        map.set(Number.parseInt(key), value)
+    }
+    return map
 }
 
 interface ModifyAttributesPatch {
     kind: 'modify-attrs'
     add: { [key: string]: any };
     remove: string[];
     element_id: string;
@@ -173,14 +187,15 @@
         if (typeof value == 'string') {
             elt.setAttribute(key, value);
         } else if ('__handler__' in value) {
             const handler_id = value['__handler__'];
             const handler = (args: any) => this.onEvent({ element_id: vn.id, handler_id, name: key, params: args })
             vn.handlers.set(key, handler)
             elt.addEventListener(key, handler)
+            console.debug('added handler', vn.node.nodeType, key, handler_id)
         } else if (key == 'style') {
             for (const sk in value) {
                 const sv = value[sk];
                 // @ts-ignore
                 elt.style[sk] = sv;
             }
         } else {
@@ -190,14 +205,15 @@
 
     rmAttr(vn: VdomNode, key: string) {
         const elt: Element = vn.node as any;
         if (vn.handlers.has(key)) {
             const handler = vn.handlers.get(key)!;
             elt.removeEventListener(key, handler)
             vn.handlers.delete(key)
+            console.debug('remove handler', vn.node.nodeType, key)
         } else {
             elt.removeAttribute(key);
         }
     }
 
     create(x: Rendering, parent_id: string): Vdom {
         if (x.kind == 'element') {
@@ -206,15 +222,17 @@
             this.setVdom(vn)
             for (const key in x.attrs) {
                 const val = x.attrs[key];
                 this.setAttr(vn, key, val);
             }
             for (const child of x.children) {
                 const cn = this.create(child, x.id)
-                elt.appendChild(cn.node);
+                if (cn.node !== elt) {
+                    elt.appendChild(cn.node);
+                }
             }
             this.setVdom(vn)
             return vn
         } else if (x.kind == 'text') {
             const text = document.createTextNode(x.value);
             const vn: VdomNode = { id: x.id, node: text, handlers: new Map(), child_ids: [], kind: 'text' }
             this.setVdom(vn);
@@ -313,38 +331,42 @@
                 const val = patch.add[key]
                 this.setAttr(vn, key, val)
             }
         }
     }
 
     modifyChildren(patch: ModifyChildrenPatch): void {
+        const remove_these = mapOfObject(patch.reorder.remove_these)
+        const then_insert_these = mapOfObject(patch.reorder.then_insert_these)
+        const l1_len = patch.reorder.l1_len
         const fidx = this.getFragmentIdx(patch.element_id)
         const vn = this.nodes.get(patch.element_id)!
         const elt: Element = vn.node as any
-        if (elt.childNodes.length < patch.children_length_start) {
-            console.error(`modifyChildren: ${elt} has ${elt.childNodes.length} children but was expected to have at least ${patch.children_length_start}`)
+        if (elt.childNodes.length < l1_len) {
+            console.error(`modifyChildren: ${elt} has ${elt.childNodes.length} children but was expected to have at least ${l1_len}`)
         }
         const cvns = vn.child_ids.map(id => this.nodes.get(id)!)
         const bucket = new Map()
-        const removals = Array.from(patch.remove_these.entries()).sort((a, b) => a[0] - b[0])
+
+        const removals = Array.from(remove_these.entries()).sort((a, b) => a[0] - b[0])
         for (const [i, v] of removals) {
             const child_node = elt.childNodes[i + fidx]
             const cvn = cvns[i]
             if (child_node !== cvn.node) {
                 throw new Error(`modifyChildren ${i}: ${child_node} is not ${cvn.node}`)
             }
             elt.removeChild(child_node)
             if (typeof v === 'string') {
                 bucket.set(v, cvn)
             } else {
                 this.remove(cvn.id)
             }
         }
-        vn.child_ids = vn.child_ids.filter((id, i) => !patch.remove_these.has(i))
-        const insertions = Array.from(patch.then_insert_these.entries()).sort((a, b) => b[0] - a[0])
+        vn.child_ids = vn.child_ids.filter((id, i) => !remove_these.has(i))
+        const insertions = Array.from(then_insert_these.entries()).sort((a, b) => b[0] - a[0])
         for (const [j, kv] of insertions) {
             const cb = (j + fidx) >= elt.childNodes.length ? null : elt.childNodes[j + fidx]
             const new_vn: VdomNode = kv[0] === 0 ? bucket.get(kv[1]) : this.create(kv[1], vn.id)
             this.setVdom(new_vn)
             elt.insertBefore(new_vn.node, cb)
             vn.child_ids.splice(j, 0, new_vn.id)
         }
```

### Comparing `uxu-0.0.2/web/src/rpc.ts` & `uxu-0.1.1/web/src/rpc.ts`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/README.md` & `uxu-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/pyproject.toml` & `uxu-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uxu-0.0.2/PKG-INFO` & `uxu-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uxu
-Version: 0.0.2
+Version: 0.1.1
 Summary: Server-side interactive HTML engine.
 Project-URL: Documentation, https://github.com/EdAyers/sss/uxu
 Project-URL: Issues, https://github.com/EdAyers/sss/issues
 Project-URL: Source, https://github.com/EdAyers/sss/uxu
 Author-email: "E.W.Ayers" <contact@edayers.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```


# Comparing `tmp/strawberry_django_plus-2.2.0.tar.gz` & `tmp/strawberry_django_plus-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-2.2.0.tar", max compression
+gzip compressed data, was "strawberry_django_plus-2.3.0.tar", max compression
```

## Comparing `strawberry_django_plus-2.2.0.tar` & `strawberry_django_plus-2.3.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1077 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/LICENSE
--rw-r--r--   0        0        0     3299 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/README.md
--rw-r--r--   0        0        0     4162 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     2950 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5554 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5751 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    26052 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3069 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1641 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1389 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0     6287 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/middlewares/debug_toolbar.py
--rw-r--r--   0        0        0        0 2023-04-11 16:08:31.132789 strawberry_django_plus-2.2.0/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    25024 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14819 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    24443 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1372 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    27509 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0    45970 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1107 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0     1445 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
--rw-r--r--   0        0        0        0 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2337 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    16988 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/type.py
--rw-r--r--   0        0        0    10174 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6924 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    12426 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    13406 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-04-11 16:08:31.136789 strawberry_django_plus-2.2.0/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     5169 1970-01-01 00:00:00.000000 strawberry_django_plus-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-04-19 21:03:34.674986 strawberry_django_plus-2.3.0/LICENSE
+-rw-r--r--   0        0        0     3299 2023-04-19 21:03:34.674986 strawberry_django_plus-2.3.0/README.md
+-rw-r--r--   0        0        0     4162 2023-04-19 21:03:34.678986 strawberry_django_plus-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2950 2023-04-19 21:03:34.678986 strawberry_django_plus-2.3.0/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5554 2023-04-19 21:03:34.678986 strawberry_django_plus-2.3.0/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5751 2023-04-19 21:03:34.678986 strawberry_django_plus-2.3.0/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    26052 2023-04-19 21:03:34.678986 strawberry_django_plus-2.3.0/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3069 2023-04-19 21:03:34.678986 strawberry_django_plus-2.3.0/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1641 2023-04-19 21:03:34.678986 strawberry_django_plus-2.3.0/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1389 2023-04-19 21:03:34.678986 strawberry_django_plus-2.3.0/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-04-19 21:03:34.678986 strawberry_django_plus-2.3.0/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     1939 2023-04-19 21:03:34.678986 strawberry_django_plus-2.3.0/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-04-19 21:03:34.678986 strawberry_django_plus-2.3.0/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-04-19 21:03:34.678986 strawberry_django_plus-2.3.0/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-04-19 21:03:34.678986 strawberry_django_plus-2.3.0/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0     6287 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/middlewares/debug_toolbar.py
+-rw-r--r--   0        0        0        0 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    25024 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14819 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    24443 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1372 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    27509 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0    47551 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1107 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0     1445 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
+-rw-r--r--   0        0        0        0 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2337 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    16988 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0    10174 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6924 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    12426 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     5865 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    13406 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      938 2023-04-19 21:03:34.682986 strawberry_django_plus-2.3.0/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     5169 1970-01-01 00:00:00.000000 strawberry_django_plus-2.3.0/PKG-INFO
```

### Comparing `strawberry_django_plus-2.2.0/LICENSE` & `strawberry_django_plus-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/README.md` & `strawberry_django_plus-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/pyproject.toml` & `strawberry_django_plus-2.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "2.2.0"
+version = "2.3.0"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
@@ -46,24 +46,24 @@
 pytest = "^7.1.2"
 pytest-cov = "^4.0.0"
 pytest-django = "^4.5.2"
 django-extensions = "^3.1.5"
 ipython = "^8.4.0"
 factory-boy = "^3.2.1"
 pytest-asyncio = "^0.21.0"
-django-debug-toolbar = "^3.2.4"
+django-debug-toolbar = "^4.0.0"
 django-choices-field = "^2.0"
 django-guardian = "^2.4.0"
 mkdocs = "^1.4.2"
 mkdocs-markdownextradata-plugin = "^0.2.5"
 mkdocs-material = "^9.0.9"
 mkdocs-minify-plugin = "^0.6.2"
 pymdown-extensions = "^9.5"
 Markdown = "^3.3.7"
-ruff = "^0.0.260"
+ruff = "^0.0.261"
 
 
 [tool.poetry.extras]
 enum = ["django-choices-field"]
 debug-toolbar = ["django-debug-toolbar"]
 
 [tool.ruff]
```

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/__init__.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/directives.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/field.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/field.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/filters.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/middlewares/debug_toolbar.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/middlewares/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/mutations/fields.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/optimizer.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/ordering.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/permissions.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/relay.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/relay.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import dataclasses
 import functools
 import inspect
 import itertools
 import math
 import sys
 import uuid
+import warnings
 from typing import (
     Any,
     Awaitable,
     Callable,
     ClassVar,
     Dict,
     ForwardRef,
@@ -241,37 +242,27 @@
         ...
 
     @overload
     def resolve_node(
         self,
         info: Info,
         *,
-        required: Literal[True] = ...,
-        ensure_type: Awaitable[Type[_T]],
-    ) -> Awaitable[_T]:
-        ...
-
-    @overload
-    def resolve_node(
-        self,
-        info: Info,
-        *,
         required: Literal[True],
         ensure_type: None = ...,
-    ) -> AwaitableOrValue["Node"]:
+    ) -> "Node":
         ...
 
     @overload
     def resolve_node(
         self,
         info: Info,
         *,
         required: bool = ...,
         ensure_type: None = ...,
-    ) -> AwaitableOrValue[Optional["Node"]]:
+    ) -> Optional["Node"]:
         ...
 
     def resolve_node(self, info, *, required=False, ensure_type=None) -> Any:
         """Resolve the type name and node id info to the node itself.
 
         Tip: When you know the expected type, calling `ensure_type` should help
         not only to enforce it, but also help with typing since it will know that,
@@ -302,19 +293,81 @@
             info=info,
             required=required or ensure_type is not None,
         )
 
         if node is not None and ensure_type is not None:
             origin = get_origin(ensure_type)
             if origin and issubclass(origin, Awaitable):
+                warnings.warn("use `aresolve_node` instead", DeprecationWarning, stacklevel=1)
                 ensure_type = get_args(ensure_type)[0]
             return aio.resolve(node, lambda n: n, info=info, ensure_type=ensure_type)
 
         return node
 
+    @overload
+    async def aresolve_node(
+        self,
+        info: Info,
+        *,
+        required: Literal[True] = ...,
+        ensure_type: Type[_T],
+    ) -> _T:
+        ...
+
+    @overload
+    async def aresolve_node(
+        self,
+        info: Info,
+        *,
+        required: Literal[True],
+        ensure_type: None = ...,
+    ) -> "Node":
+        ...
+
+    @overload
+    async def aresolve_node(
+        self,
+        info: Info,
+        *,
+        required: bool = ...,
+        ensure_type: None = ...,
+    ) -> Optional["Node"]:
+        ...
+
+    async def aresolve_node(self, info, *, required=False, ensure_type=None) -> Any:
+        """Resolve the type name and node id info to the node itself.
+
+        Tip: When you know the expected type, calling `ensure_type` should help
+        not only to enforce it, but also help with typing since it will know that,
+        if this function returns successfully, the retval should be of that
+        type and not `Node`.
+
+        Args:
+            info:
+                The strawberry execution info resolve the type name from
+            required:
+                If the value is required to exist. Note that asking to ensure
+                the type automatically makes required true.
+            ensure_type:
+                Optionally check if the returned node is really an instance
+                of this type.
+
+        Returns:
+            The resolved node
+
+        Raises:
+            TypeError:
+                If ensure_type was provided and the type is not an instance of it
+
+        """
+        return await cast(
+            Awaitable,
+            self.resolve_node(info, required=required, ensure_type=ensure_type),
+        )
+
 
 # Register our GlobalID scalar
 DEFAULT_SCALAR_REGISTRY[GlobalID] = ScalarDefinition(
     # Use the same name/description/parse_literal from GraphQLID as relay
     # specs expect this type to be "ID".
     name="GlobalID",
     description=GraphQLID.description,
```

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/settings.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html` & `strawberry_django_plus-2.3.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/test/client.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/test/client.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/type.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/type.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/types.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/utils/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-2.3.0/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.2.0/PKG-INFO` & `strawberry_django_plus-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 2.2.0
+Version: 2.3.0
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```


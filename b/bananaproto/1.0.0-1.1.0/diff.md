# Comparing `tmp/bananaproto-1.0.0.tar.gz` & `tmp/bananaproto-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bananaproto-1.0.0.tar", max compression
+gzip compressed data, was "bananaproto-1.1.0.tar", max compression
```

## Comparing `bananaproto-1.0.0.tar` & `bananaproto-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    16060 2023-04-06 08:18:27.222794 bananaproto-1.0.0/README.md
--rw-r--r--   0        0        0     3369 2023-04-06 08:18:27.222794 bananaproto-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    56436 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/__init__.py
--rw-r--r--   0        0        0      295 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/_types.py
--rw-r--r--   0        0        0       99 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/_version.py
--rw-r--r--   0        0        0     3543 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/casing.py
--rw-r--r--   0        0        0        0 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/compile/__init__.py
--rw-r--r--   0        0        0     6337 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/compile/importing.py
--rw-r--r--   0        0        0      286 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/compile/naming.py
--rw-r--r--   0        0        0        0 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/grpc/__init__.py
--rw-r--r--   0        0        0     5295 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/grpc/grpclib_client.py
--rw-r--r--   0        0        0      882 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/grpc/grpclib_server.py
--rw-r--r--   0        0        0        0 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/grpc/util/__init__.py
--rw-r--r--   0        0        0     6793 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/grpc/util/async_channel.py
--rw-r--r--   0        0        0        0 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/lib/google/__init__.py
--rw-r--r--   0        0        0    70836 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/lib/google/protobuf/__init__.py
--rw-r--r--   0        0        0     7057 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/lib/google/protobuf/compiler/__init__.py
--rw-r--r--   0        0        0       23 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/plugin/__init__.py
--rw-r--r--   0        0        0       32 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/plugin/__main__.py
--rw-r--r--   0        0        0     1320 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/plugin/compiler.py
--rwxr-xr-x   0        0        0     1471 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/plugin/main.py
--rw-r--r--   0        0        0    28144 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/plugin/models.py
--rw-r--r--   0        0        0     7649 2023-04-06 08:18:27.222794 bananaproto-1.0.0/src/bananaproto/plugin/parser.py
--rw-r--r--   0        0        0       48 2023-04-06 08:18:27.226794 bananaproto-1.0.0/src/bananaproto/plugin/plugin.bat
--rw-r--r--   0        0        0        0 2023-04-06 08:18:27.226794 bananaproto-1.0.0/src/bananaproto/py.typed
--rw-r--r--   0        0        0     8713 2023-04-06 08:18:27.226794 bananaproto-1.0.0/src/bananaproto/templates/template.py.j2
--rw-r--r--   0        0        0    17169 1970-01-01 00:00:00.000000 bananaproto-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    16280 2023-04-19 00:24:54.144058 bananaproto-1.1.0/README.md
+-rw-r--r--   0        0        0     3369 2023-04-19 00:24:54.144058 bananaproto-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    56436 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/__init__.py
+-rw-r--r--   0        0        0      295 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/_types.py
+-rw-r--r--   0        0        0       99 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/_version.py
+-rw-r--r--   0        0        0     3543 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/casing.py
+-rw-r--r--   0        0        0        0 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/compile/__init__.py
+-rw-r--r--   0        0        0     6337 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/compile/importing.py
+-rw-r--r--   0        0        0      286 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/compile/naming.py
+-rw-r--r--   0        0        0        0 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/grpc/__init__.py
+-rw-r--r--   0        0        0     5295 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/grpc/grpclib_client.py
+-rw-r--r--   0        0        0      982 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/grpc/grpclib_server.py
+-rw-r--r--   0        0        0        0 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/grpc/util/__init__.py
+-rw-r--r--   0        0        0     6793 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/grpc/util/async_channel.py
+-rw-r--r--   0        0        0        0 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-19 00:24:54.144058 bananaproto-1.1.0/src/bananaproto/lib/google/__init__.py
+-rw-r--r--   0        0        0    70836 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/lib/google/protobuf/__init__.py
+-rw-r--r--   0        0        0     7057 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/lib/google/protobuf/compiler/__init__.py
+-rw-r--r--   0        0        0       23 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/__init__.py
+-rw-r--r--   0        0        0       32 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/__main__.py
+-rw-r--r--   0        0        0     1320 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/compiler.py
+-rwxr-xr-x   0        0        0     1471 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/main.py
+-rw-r--r--   0        0        0    28084 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/models.py
+-rw-r--r--   0        0        0     7649 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/parser.py
+-rw-r--r--   0        0        0       48 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/plugin/plugin.bat
+-rw-r--r--   0        0        0        0 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/py.typed
+-rw-r--r--   0        0        0     8391 2023-04-19 00:24:54.148058 bananaproto-1.1.0/src/bananaproto/templates/template.py.j2
+-rw-r--r--   0        0        0    17389 1970-01-01 00:00:00.000000 bananaproto-1.1.0/PKG-INFO
```

### Comparing `bananaproto-1.0.0/README.md` & `bananaproto-1.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -382,15 +382,14 @@
 pydantic dataclass. You must have pydantic as a dependency in your project for
 this to work.
 
 
 
 ## Development
 
-- _Join us on [Slack](https://join.slack.com/t/betterproto/shared_invite/zt-f0n0uolx-iN8gBNrkPxtKHTLpG3o1OQ)!_
 - _See how you can help &rarr; [Contributing](.github/CONTRIBUTING.md)_
 
 ### Requirements
 
 - Python (3.7 or higher)
 
 - [poetry](https://python-poetry.org/docs/#installation)
@@ -516,12 +515,23 @@
   - [x] Client streaming request
 - [x] Renaming messages and fields to conform to Python name standards
 - [x] Renaming clashes with language keywords
 - [x] Python package
 - [x] Automate running tests
 - [ ] Cleanup!
 
+### Banana TODO
+
+- [x] Fix input types imports
+- [x] Non-string type hint
+- [ ] Add *Reflections* chapter to README
+- [ ] Return original folder structure
+  - [ ] Automatically import *_pb2 for reflections
+- [x] Pass metadata to Service methods
+- [ ] Fix comments in generated code
+- [ ] Omit Empty argument from Stub and Service
+
 ## License
 
 Copyright © 2019 Daniel G. Taylor
 
 http://dgt.mit-license.org/
```

### Comparing `bananaproto-1.0.0/pyproject.toml` & `bananaproto-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bananaproto"
-version = "1.0.0"
+version = "1.1.0"
 description = "A BANANA Protobuf / gRPC generator & library"
 authors = ["Daniel G. Taylor <danielgtaylor@gmail.com>"]
 maintainers = ["BananaLoaf <bananaloaf@protonmail.com>"]
 readme = "README.md"
 repository = "https://github.com/BananaLoaf/python-bananaproto"
 keywords = ["protobuf", "gRPC"]
 license = "MIT"
```

### Comparing `bananaproto-1.0.0/src/bananaproto/__init__.py` & `bananaproto-1.1.0/src/bananaproto/__init__.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.0.0/src/bananaproto/casing.py` & `bananaproto-1.1.0/src/bananaproto/casing.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.0.0/src/bananaproto/compile/importing.py` & `bananaproto-1.1.0/src/bananaproto/compile/importing.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.0.0/src/bananaproto/grpc/grpclib_client.py` & `bananaproto-1.1.0/src/bananaproto/grpc/grpclib_client.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.0.0/src/bananaproto/grpc/grpclib_server.py` & `bananaproto-1.1.0/src/bananaproto/grpc/grpclib_server.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,27 +5,30 @@
     Callable,
     Dict,
 )
 
 import grpclib
 import grpclib.server
 
+from bananaproto.grpc.grpclib_client import MetadataLike
+
 
 class ServiceBase(ABC):
     """
     Base class for async gRPC servers.
     """
 
     async def _call_rpc_handler_server_stream(
         self,
         handler: Callable,
         stream: grpclib.server.Stream,
         request: Any,
+        metadata: MetadataLike,
     ) -> None:
-        response_iter = handler(request)
+        response_iter = handler(request, metadata)
         # check if response is actually an AsyncIterator
         # this might be false if the method just returns without
         # yielding at least once
         # in that case, we just interpret it as an empty iterator
         if isinstance(response_iter, AsyncIterable):
             async for response_message in response_iter:
                 await stream.send_message(response_message)
```

### Comparing `bananaproto-1.0.0/src/bananaproto/grpc/util/async_channel.py` & `bananaproto-1.1.0/src/bananaproto/grpc/util/async_channel.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.0.0/src/bananaproto/lib/google/protobuf/__init__.py` & `bananaproto-1.1.0/src/bananaproto/lib/google/protobuf/__init__.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.0.0/src/bananaproto/lib/google/protobuf/compiler/__init__.py` & `bananaproto-1.1.0/src/bananaproto/lib/google/protobuf/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.0.0/src/bananaproto/plugin/compiler.py` & `bananaproto-1.1.0/src/bananaproto/plugin/compiler.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.0.0/src/bananaproto/plugin/main.py` & `bananaproto-1.1.0/src/bananaproto/plugin/main.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.0.0/src/bananaproto/plugin/models.py` & `bananaproto-1.1.0/src/bananaproto/plugin/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -737,20 +737,18 @@
         # Required by both client and server
         if self.client_streaming or self.server_streaming:
             self.output_file.typing_imports.add("AsyncIterator")
 
         # add imports required for request arguments timeout, deadline and metadata
         self.output_file.typing_imports.add("Optional")
         self.output_file.imports_type_checking_only.add("import grpclib.server")
-        self.output_file.imports_type_checking_only.add(
+        self.output_file.imports.add(
             "from bananaproto.grpc.grpclib_client import MetadataLike"
         )
-        self.output_file.imports_type_checking_only.add(
-            "from grpclib.metadata import Deadline"
-        )
+        self.output_file.imports.add("from grpclib.metadata import Deadline")
 
         super().__post_init__()  # check for unset fields
 
     @property
     def py_name(self) -> str:
         """Pythonized method name."""
         return pythonize_method_name(self.proto_obj.name)
```

### Comparing `bananaproto-1.0.0/src/bananaproto/plugin/parser.py` & `bananaproto-1.1.0/src/bananaproto/plugin/parser.py`

 * *Files identical despite different names*

### Comparing `bananaproto-1.0.0/src/bananaproto/templates/template.py.j2` & `bananaproto-1.1.0/src/bananaproto/templates/template.py.j2`

 * *Files 14% similar despite different names*

```diff
@@ -107,70 +107,69 @@
     {% if service.comment %}
 {{ service.comment }}
 
     {% elif not service.methods %}
     pass
     {% endif %}
     {% for method in service.methods %}
-    async def {{ method.py_name }}(self
+    async def {{ method.py_name }}(self,
         {%- if not method.client_streaming -%}
-            {%- if method.py_input_message -%}, {{ method.py_input_message_param }}: {{ method.py_input_message_type }}{%- endif -%}
+            {%- if method.py_input_message -%} msg: {{ method.py_input_message_type }}, {%- endif -%}
         {%- else -%}
             {# Client streaming: need a request iterator instead #}
-            , {{ method.py_input_message_param }}_iterator: Union[AsyncIterable[{{ method.py_input_message_type }}], Iterable[{{ method.py_input_message_type }}]]
+            msg_iter: Union[AsyncIterable[{{ method.py_input_message_type }}], Iterable[{{ method.py_input_message_type }}]],
         {%- endif -%}
-            ,
-            *
-            , timeout: Optional[float] = None
-            , deadline: Optional["Deadline"] = None
-            , metadata: Optional["MetadataLike"] = None
+            *,
+            timeout: Optional[float] = None,
+            deadline: Optional[Deadline] = None,
+            metadata: Optional[MetadataLike] = None,
             ) -> {% if method.server_streaming %}AsyncIterator[{{ method.py_output_message_type }}]{% else %}{{ method.py_output_message_type }}{% endif %}:
         {% if method.comment %}
 {{ method.comment }}
 
         {% endif %}
         {% if method.server_streaming %}
             {% if method.client_streaming %}
         async for response in self._stream_stream(
             "{{ method.route }}",
-            {{ method.py_input_message_param }}_iterator,
+            msg_iter,
             {{ method.py_input_message_type }},
             {{ method.py_output_message_type.strip('"') }},
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
             {% else %}{# i.e. not client streaming #}
         async for response in self._unary_stream(
             "{{ method.route }}",
-            {{ method.py_input_message_param }},
+            msg,
             {{ method.py_output_message_type.strip('"') }},
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         ):
             yield response
 
             {% endif %}{# if client streaming #}
         {% else %}{# i.e. not server streaming #}
             {% if method.client_streaming %}
         return await self._stream_unary(
             "{{ method.route }}",
-            {{ method.py_input_message_param }}_iterator,
+            msg_iter,
             {{ method.py_input_message_type }},
             {{ method.py_output_message_type.strip('"') }},
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
             {% else %}{# i.e. not client streaming #}
         return await self._unary_unary(
             "{{ method.route }}",
-            {{ method.py_input_message_param }},
+            msg,
             {{ method.py_output_message_type.strip('"') }},
             timeout=timeout,
             deadline=deadline,
             metadata=metadata,
         )
             {% endif %}{# client streaming #}
         {% endif %}
@@ -182,48 +181,47 @@
 class {{ service.py_name }}Base(ServiceBase):
     {% if service.comment %}
 {{ service.comment }}
 
     {% endif %}
 
     {% for method in service.methods %}
-    async def {{ method.py_name }}(self
+    async def {{ method.py_name }}(self,
         {%- if not method.client_streaming -%}
-            {%- if method.py_input_message -%}, {{ method.py_input_message_param }}: {{ method.py_input_message_type }}{%- endif -%}
+            {%- if method.py_input_message -%}msg: {{ method.py_input_message_type }}, {%- endif -%}
         {%- else -%}
             {# Client streaming: need a request iterator instead #}
-            , {{ method.py_input_message_param }}_iterator: AsyncIterator[{{ method.py_input_message_type }}]
+            msg_iter: AsyncIterator[{{ method.py_input_message_type }}],
         {%- endif -%}
+            metadata: MetadataLike,
             ) -> {% if method.server_streaming %}AsyncIterator[{{ method.py_output_message_type }}]{% else %}{{ method.py_output_message_type }}{% endif %}:
         {% if method.comment %}
 {{ method.comment }}
 
         {% endif %}
         raise grpclib.GRPCError(grpclib.const.Status.UNIMPLEMENTED)
-        {% if method.server_streaming %}
-        yield {{ method.py_output_message_type }}()
-        {% endif %}
 
     {% endfor %}
 
     {% for method in service.methods %}
     async def __rpc_{{ method.py_name }}(self, stream: grpclib.server.Stream[{{ method.py_input_message_type }}, {{ method.py_output_message_type }}]) -> None:
         {% if not method.client_streaming %}
         request = await stream.recv_message()
         {% else %}
         request = stream.__aiter__()
         {% endif %}
         {% if not method.server_streaming %}
-        response = await self.{{ method.py_name }}(request)
+        response = await self.{{ method.py_name }}(request, stream.metadata)
         await stream.send_message(response)
         {% else %}
         await self._call_rpc_handler_server_stream(
             self.{{ method.py_name }},
             stream,
             request,
+            stream.metadata,
         )
         {% endif %}
 
     {% endfor %}
 
     def __mapping__(self) -> Dict[str, grpclib.const.Handler]:
         return {
```

### Comparing `bananaproto-1.0.0/PKG-INFO` & `bananaproto-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bananaproto
-Version: 1.0.0
+Version: 1.1.0
 Summary: A BANANA Protobuf / gRPC generator & library
 Home-page: https://github.com/BananaLoaf/python-bananaproto
 License: MIT
 Keywords: protobuf,gRPC
 Author: Daniel G. Taylor
 Author-email: danielgtaylor@gmail.com
 Maintainer: BananaLoaf
@@ -410,15 +410,14 @@
 pydantic dataclass. You must have pydantic as a dependency in your project for
 this to work.
 
 
 
 ## Development
 
-- _Join us on [Slack](https://join.slack.com/t/betterproto/shared_invite/zt-f0n0uolx-iN8gBNrkPxtKHTLpG3o1OQ)!_
 - _See how you can help &rarr; [Contributing](.github/CONTRIBUTING.md)_
 
 ### Requirements
 
 - Python (3.7 or higher)
 
 - [poetry](https://python-poetry.org/docs/#installation)
@@ -544,13 +543,24 @@
   - [x] Client streaming request
 - [x] Renaming messages and fields to conform to Python name standards
 - [x] Renaming clashes with language keywords
 - [x] Python package
 - [x] Automate running tests
 - [ ] Cleanup!
 
+### Banana TODO
+
+- [x] Fix input types imports
+- [x] Non-string type hint
+- [ ] Add *Reflections* chapter to README
+- [ ] Return original folder structure
+  - [ ] Automatically import *_pb2 for reflections
+- [x] Pass metadata to Service methods
+- [ ] Fix comments in generated code
+- [ ] Omit Empty argument from Stub and Service
+
 ## License
 
 Copyright © 2019 Daniel G. Taylor
 
 http://dgt.mit-license.org/
```


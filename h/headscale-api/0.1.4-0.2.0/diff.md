# Comparing `tmp/headscale_api-0.1.4.tar.gz` & `tmp/headscale_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "headscale_api-0.1.4.tar", max compression
+gzip compressed data, was "headscale_api-0.2.0.tar", max compression
```

## Comparing `headscale_api-0.1.4.tar` & `headscale_api-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-04-17 12:42:47.464949 headscale_api-0.1.4/LICENSE
--rw-r--r--   0        0        0       68 2023-04-17 12:42:47.464949 headscale_api-0.1.4/README.md
--rw-r--r--   0        0        0      537 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/__init__.py
--rw-r--r--   0        0        0      428 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/config.py
--rw-r--r--   0        0        0     9775 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/endpoints.py
--rw-r--r--   0        0        0     7084 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/headscale.py
--rw-r--r--   0        0        0        0 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/py.typed
--rw-r--r--   0        0        0        0 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/schema/__init__.py
--rw-r--r--   0        0        0     3967 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/schema/config.py
--rw-r--r--   0        0        0        0 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/schema/google/__init__.py
--rw-r--r--   0        0        0    15302 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/schema/google/api/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/schema/headscale/__init__.py
--rw-r--r--   0        0        0    48177 2023-04-17 12:42:47.464949 headscale_api-0.1.4/headscale_api/schema/headscale/v1/__init__.py
--rw-r--r--   0        0        0     1887 2023-04-17 12:42:47.464949 headscale_api-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 headscale_api-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-18 22:43:24.116719 headscale_api-0.2.0/LICENSE
+-rw-r--r--   0        0        0       68 2023-04-18 22:43:24.116719 headscale_api-0.2.0/README.md
+-rw-r--r--   0        0        0      537 2023-04-18 22:43:24.116719 headscale_api-0.2.0/headscale_api/__init__.py
+-rw-r--r--   0        0        0      428 2023-04-18 22:43:24.116719 headscale_api-0.2.0/headscale_api/config.py
+-rw-r--r--   0        0        0     9775 2023-04-18 22:43:24.116719 headscale_api-0.2.0/headscale_api/endpoints.py
+-rw-r--r--   0        0        0     7770 2023-04-18 22:43:24.116719 headscale_api-0.2.0/headscale_api/headscale.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:43:24.116719 headscale_api-0.2.0/headscale_api/py.typed
+-rw-r--r--   0        0        0        0 2023-04-18 22:43:24.116719 headscale_api-0.2.0/headscale_api/schema/__init__.py
+-rw-r--r--   0        0        0     3967 2023-04-18 22:43:24.116719 headscale_api-0.2.0/headscale_api/schema/config.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:43:24.116719 headscale_api-0.2.0/headscale_api/schema/google/__init__.py
+-rw-r--r--   0        0        0    15302 2023-04-18 22:43:24.116719 headscale_api-0.2.0/headscale_api/schema/google/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 22:43:24.116719 headscale_api-0.2.0/headscale_api/schema/headscale/__init__.py
+-rw-r--r--   0        0        0    48771 2023-04-18 22:43:24.116719 headscale_api-0.2.0/headscale_api/schema/headscale/v1/__init__.py
+-rw-r--r--   0        0        0     1900 2023-04-18 22:43:24.120719 headscale_api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1010 1970-01-01 00:00:00.000000 headscale_api-0.2.0/PKG-INFO
```

### Comparing `headscale_api-0.1.4/LICENSE` & `headscale_api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.4/headscale_api/__init__.py` & `headscale_api-0.2.0/headscale_api/__init__.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.4/headscale_api/endpoints.py` & `headscale_api-0.2.0/headscale_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.4/headscale_api/headscale.py` & `headscale_api-0.2.0/headscale_api/headscale.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,106 @@
 """Headscale API abstraction."""
 
 __authors__ = ["Marek Pikuła <marek@serenitycode.dev>"]
 
+import json
 import logging
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
 from json import JSONDecodeError
-from typing import Any, Dict, Generator, List, Optional, Tuple, Type, TypeVar, Union
+from typing import Any, Dict, List, Optional, Tuple, Type, TypeVar, Union
 
 import requests
 from betterproto import Message
-from betterproto.casing import safe_snake_case
 
 from .endpoints import ENDPOINTS, Endpoint
 from .schema.headscale import v1 as model
 
+Response = Tuple[str, int]
+"""Response in form acceptable by Flask.
+
+`(response: str, status: int)`
+"""
+
 
 @dataclass
-class ErrorResponse(RuntimeError):
+class ResponseError(RuntimeError):
     """Error response from Headscale."""
 
-    code: int
+    http_code: int
+    """HTTP code of error."""
+
+    code: Optional[int]
+    """Error code from server."""
+
     message: str
+    """Error message."""
+
     details: List[str]
+    """Error details."""
 
     def __str__(self) -> str:  # noqa
         return f"Response (code {self.code}): {self.message}"
 
+    def to_reponse(self) -> Response:
+        """Make a Flask-compatible error response."""
+        return json.dumps(asdict(self)), self.http_code
+
+    def raise_or_respond(
+        self, raise_exception: bool, source_exception: Optional[BaseException] = None
+    ) -> "Response":
+        """Raise exception or gracefully return response.
+
+        Arguments:
+            raise_exception -- raise exception instead of gracefully returning.
+            source_exception -- exception which triggered this error.
+
+        Raises:
+            ResponseError: if `raise_exception` is set.
+
+        Returns:
+            Flask-compatible response if `raise_exception` is False.
+        """
+        if raise_exception:
+            raise self from source_exception
+        return self.to_reponse()
+
 
 MessageT = TypeVar("MessageT", bound=Message)
 """Message type for Headscale._unary_unary() function."""
 
 
 class Headscale(model.HeadscaleServiceStub):
     """Headscale API abstraction."""
 
-    def __init__(  # pylint: disable=super-init-not-called
+    def __init__(  # pylint: disable=super-init-not-called,too-many-arguments
         self,
         base_url: str,
         api_key: Optional[str] = None,
         requests_timeout: float = 10,
+        raise_exception_on_error: bool = True,
         logger: Union[logging.Logger, int] = logging.INFO,
     ):
         """Initialize Headscale API.
 
         Arguments:
             base_url -- base API URL (without `/api/v1`).
 
         Keyword Arguments:
             api_key -- API key, which can be overriden later (default: {None})
             requests_timeout -- request timeout in seconds (default: {10})
+            raise_exception_on_error -- raise exception in error (eiher internal or from
+                the API). Otherwise, return Flask-compatible response tuple
+                (default: {True})
             logger -- logger to use or default logging level
                 (default: {logging.INFO})
         """
         self._base_url = base_url
         self._api_key = api_key
         self.timeout = requests_timeout
+        self.raise_exception_on_error = raise_exception_on_error
         if isinstance(logger, logging.Logger):
             self._logger = logger
         else:
             logging.basicConfig(level=logger)
             self._logger = logging.getLogger(__name__)
 
     @property
@@ -107,47 +149,24 @@
     async def health_check(self) -> bool:
         """Perform a health check.
 
         Returns True if check passed.
         """
         return requests.get(self.health_url, timeout=self.timeout).status_code == 200
 
-    def _safe_snake_case_recursive(
-        self, dictionary: Dict[str, Any]
-    ) -> Generator[Tuple[str, Any], None, None]:
-        assert isinstance(dictionary, dict)
-        for key, value in dictionary.items():
-            escaped_key = safe_snake_case(key)
-            if isinstance(value, dict):
-                yield (
-                    escaped_key,
-                    dict(self._safe_snake_case_recursive(value)),  # type: ignore
-                )
-            elif isinstance(value, list):
-                yield escaped_key, list(
-                    list_value
-                    if not isinstance(list_value, dict)
-                    else dict(
-                        self._safe_snake_case_recursive(list_value)  # type: ignore
-                    )
-                    for list_value in value  # type: ignore
-                )
-            else:
-                yield escaped_key, value
-
     async def _unary_unary(  # type: ignore
         self,
         route: str,
         request: Message,
         response_type: Type[MessageT],
         *,
         timeout: Optional[Any] = None,
         deadline: Optional[Any] = None,
         metadata: Optional[Any] = None,
-    ) -> MessageT:
+    ) -> Union[MessageT, Response]:
         """Execute an unary operation on the API.
 
         Used by HeadscaleServiceStub functions.
         """
         try:
             endpoint = ENDPOINTS[route]
             assert isinstance(endpoint, Endpoint)
@@ -179,33 +198,38 @@
             ) + f" ({response.status_code})"  # type: ignore
             self._logger.error(message)
             return message
 
         if response.status_code != 200:
             error_message()
             try:
-                raise ErrorResponse(**response.json())
+                return ResponseError(
+                    http_code=response.status_code, **response.json()
+                ).raise_or_respond(self.raise_exception_on_error)
             except JSONDecodeError as error:
-                raise ErrorResponse(
-                    response.status_code, response.content.decode(), []
-                ) from error
+                return ResponseError(
+                    response.status_code, None, response.content.decode(), []
+                ).raise_or_respond(self.raise_exception_on_error, error)
 
         try:
-            response_dict = dict(self._safe_snake_case_recursive(response.json()))
-            response_parsed = response_type(**response_dict)  # type: ignore
+            response_parsed: MessageT = response_type.from_dict(  # type: ignore
+                response.json()
+            )
         except (JSONDecodeError, AssertionError, ValueError) as error:
-            raise ErrorResponse(response.status_code, error_message(), []) from error
+            return ResponseError(500, 0, error_message(), []).raise_or_respond(
+                self.raise_exception_on_error, error
+            )
 
         if endpoint.logger_success_message is not None:
             self._logger.info(
                 endpoint.logger_success_message.format_map(
-                    dict(request_dict, **response_dict)
+                    dict(request_dict, **response_parsed.to_dict())  # type: ignore
                 )
             )
-        return response_parsed
+        return response_parsed  # type: ignore
 
     async def _unary_stream(  # type: ignore
         self,
         route: str,
         request: Any,
         response_type: Any,
         *,
```

### Comparing `headscale_api-0.1.4/headscale_api/schema/config.py` & `headscale_api-0.2.0/headscale_api/schema/config.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.4/headscale_api/schema/google/api/__init__.py` & `headscale_api-0.2.0/headscale_api/schema/google/api/__init__.py`

 * *Files identical despite different names*

### Comparing `headscale_api-0.1.4/headscale_api/schema/headscale/v1/__init__.py` & `headscale_api-0.2.0/headscale_api/schema/headscale/v1/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 # sources: headscale/v1/apikey.proto, headscale/v1/device.proto, headscale/v1/headscale.proto, headscale/v1/machine.proto, headscale/v1/preauthkey.proto, headscale/v1/routes.proto, headscale/v1/user.proto
 # plugin: python-betterproto
 # This file has been @generated
 
 from typing import TYPE_CHECKING
 
 
-from pydantic.dataclasses import dataclass
+if TYPE_CHECKING:
+    from dataclasses import dataclass
+else:
+    from pydantic.dataclasses import dataclass
 
 from datetime import datetime
 from typing import (
     TYPE_CHECKING,
     Dict,
     List,
     Optional,
 )
 
 import betterproto
 import grpclib
 from betterproto.grpc.grpclib_server import ServiceBase
+from pydantic import root_validator
 
 
 if TYPE_CHECKING:
     import grpclib.server
     from betterproto.grpc.grpclib_client import MetadataLike
     from grpclib.metadata import Deadline
 
@@ -36,15 +40,21 @@
 
 @dataclass(eq=False, repr=False)
 class ApiKey(betterproto.Message):
     id: int = betterproto.uint64_field(1)
     prefix: str = betterproto.string_field(2)
     expiration: datetime = betterproto.message_field(3)
     created_at: datetime = betterproto.message_field(4)
-    last_seen: Optional[datetime] = betterproto.message_field(5)
+    last_seen: Optional[datetime] = betterproto.message_field(
+        5, optional=True, group="_last_seen"
+    )
+
+    @root_validator()
+    def check_oneof(cls, values):
+        return cls._validate_field_groups(values)
 
 
 @dataclass(eq=False, repr=False)
 class CreateApiKeyRequest(betterproto.Message):
     expiration: datetime = betterproto.message_field(1)
 
 
@@ -276,23 +286,29 @@
     disco_key: str = betterproto.string_field(4)
     ip_addresses: List[str] = betterproto.string_field(5)
     name: str = betterproto.string_field(6)
     user: "User" = betterproto.message_field(7)
     last_seen: datetime = betterproto.message_field(8)
     last_successful_update: datetime = betterproto.message_field(9)
     expiry: datetime = betterproto.message_field(10)
-    pre_auth_key: "PreAuthKey" = betterproto.message_field(11)
+    pre_auth_key: Optional["PreAuthKey"] = betterproto.message_field(
+        11, optional=True, group="_pre_auth_key"
+    )
     created_at: datetime = betterproto.message_field(12)
     register_method: "RegisterMethod" = betterproto.enum_field(13)
     forced_tags: List[str] = betterproto.string_field(18)
     invalid_tags: List[str] = betterproto.string_field(19)
     valid_tags: List[str] = betterproto.string_field(20)
     given_name: str = betterproto.string_field(21)
     online: bool = betterproto.bool_field(22)
 
+    @root_validator()
+    def check_oneof(cls, values):
+        return cls._validate_field_groups(values)
+
 
 @dataclass(eq=False, repr=False)
 class RegisterMachineRequest(betterproto.Message):
     user: str = betterproto.string_field(1)
     key: str = betterproto.string_field(2)
 
 
@@ -393,15 +409,21 @@
     machine: "Machine" = betterproto.message_field(2)
     prefix: str = betterproto.string_field(3)
     advertised: bool = betterproto.bool_field(4)
     enabled: bool = betterproto.bool_field(5)
     is_primary: bool = betterproto.bool_field(6)
     created_at: datetime = betterproto.message_field(7)
     updated_at: datetime = betterproto.message_field(8)
-    deleted_at: datetime = betterproto.message_field(9)
+    deleted_at: Optional[datetime] = betterproto.message_field(
+        9, optional=True, group="_deleted_at"
+    )
+
+    @root_validator()
+    def check_oneof(cls, values):
+        return cls._validate_field_groups(values)
 
 
 @dataclass(eq=False, repr=False)
 class GetRoutesRequest(betterproto.Message):
     pass
```

### Comparing `headscale_api-0.1.4/pyproject.toml` & `headscale_api-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "headscale-api"
-version = "0.1.4"
+version = "0.2.0"
 description = "Python Headscale API and configuration abstraction."
 authors = ["Marek Pikuła <marek@serenitycode.dev>"]
 maintainers = ["Marek Pikuła <marek@serenitycode.dev>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -42,15 +42,15 @@
 pylint-pytest = "^1.1.2"
 
 [tool.poetry.group.gen.dependencies]
 datamodel-code-generator = "^0.17.2"
 
 [tool.poetry.group.dev.dependencies]
 # Add direct dependency only for development.
-betterproto = {git = "https://github.com/danielgtaylor/python-betterproto.git", rev = "master", extras = ["compiler"]}
+betterproto = {git = "https://github.com/MarekPikula/python-betterproto.git", rev = "classmethod_from_dict", extras = ["compiler"]}
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `headscale_api-0.1.4/PKG-INFO` & `headscale_api-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: headscale-api
-Version: 0.1.4
+Version: 0.2.0
 Summary: Python Headscale API and configuration abstraction.
 Home-page: https://github.com/MarekPikula/python-headscale-api
 License: MIT
 Author: Marek Pikuła
 Author-email: marek@serenitycode.dev
 Maintainer: Marek Pikuła
 Maintainer-email: marek@serenitycode.dev
```


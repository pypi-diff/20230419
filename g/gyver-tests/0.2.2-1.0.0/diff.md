# Comparing `tmp/gyver_tests-0.2.2.tar.gz` & `tmp/gyver_tests-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyver_tests-0.2.2.tar", max compression
+gzip compressed data, was "gyver_tests-1.0.0.tar", max compression
```

## Comparing `gyver_tests-0.2.2.tar` & `gyver_tests-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0        0 2023-01-30 18:25:08.989664 gyver_tests-0.2.2/README.md
--rw-r--r--   0        0        0        0 2023-01-30 19:00:44.025644 gyver_tests-0.2.2/gyver/tests/__init__.py
--rw-r--r--   0        0        0       61 2023-02-02 10:35:06.588515 gyver_tests-0.2.2/gyver/tests/config/__init__.py
--rw-r--r--   0        0        0     5193 2023-02-02 20:32:31.043616 gyver_tests-0.2.2/gyver/tests/config/mocker.py
--rw-r--r--   0        0        0     1901 2023-02-02 20:32:31.046949 gyver_tests-0.2.2/gyver/tests/config/registry.py
--rw-r--r--   0        0        0       83 2023-01-31 21:24:40.061171 gyver_tests-0.2.2/gyver/tests/http/__init__.py
--rw-r--r--   0        0        0      582 2023-01-31 20:57:26.798283 gyver_tests-0.2.2/gyver/tests/http/exc.py
--rw-r--r--   0        0        0      997 2023-01-31 22:15:33.212203 gyver_tests-0.2.2/gyver/tests/http/helpers.py
--rw-r--r--   0        0        0    10136 2023-02-02 20:32:30.583604 gyver_tests-0.2.2/gyver/tests/http/mocker.py
--rw-r--r--   0        0        0     2715 2023-01-31 22:15:33.765549 gyver_tests-0.2.2/gyver/tests/http/mocker.pyi
--rw-r--r--   0        0        0      573 2023-01-31 21:24:50.211382 gyver_tests-0.2.2/gyver/tests/http/plugin.py
--rw-r--r--   0        0        0     2176 2023-01-31 22:15:33.762215 gyver_tests-0.2.2/gyver/tests/http/typedef.py
--rw-r--r--   0        0        0      617 2023-02-02 20:33:25.024612 gyver_tests-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 gyver_tests-0.2.2/setup.py
--rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 gyver_tests-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-19 15:31:44.057551 gyver_tests-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-19 15:31:44.057551 gyver_tests-1.0.0/gyver/tests/__init__.py
+-rw-r--r--   0        0        0       61 2023-04-19 15:31:44.057551 gyver_tests-1.0.0/gyver/tests/config/__init__.py
+-rw-r--r--   0        0        0     5163 2023-04-19 16:16:19.222251 gyver_tests-1.0.0/gyver/tests/config/mocker.py
+-rw-r--r--   0        0        0     1613 2023-04-19 16:16:16.409286 gyver_tests-1.0.0/gyver/tests/config/registry.py
+-rw-r--r--   0        0        0       83 2023-04-19 15:31:44.057551 gyver_tests-1.0.0/gyver/tests/http/__init__.py
+-rw-r--r--   0        0        0      582 2023-04-19 15:31:44.057551 gyver_tests-1.0.0/gyver/tests/http/exc.py
+-rw-r--r--   0        0        0      997 2023-04-19 15:31:44.057551 gyver_tests-1.0.0/gyver/tests/http/helpers.py
+-rw-r--r--   0        0        0    10135 2023-04-19 16:16:15.848293 gyver_tests-1.0.0/gyver/tests/http/mocker.py
+-rw-r--r--   0        0        0     2715 2023-04-19 15:31:44.057551 gyver_tests-1.0.0/gyver/tests/http/mocker.pyi
+-rw-r--r--   0        0        0      573 2023-04-19 15:31:44.057551 gyver_tests-1.0.0/gyver/tests/http/plugin.py
+-rw-r--r--   0        0        0     2175 2023-04-19 16:16:15.856293 gyver_tests-1.0.0/gyver/tests/http/typedef.py
+-rw-r--r--   0        0        0      617 2023-04-19 16:16:48.521883 gyver_tests-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      518 1970-01-01 00:00:00.000000 gyver_tests-1.0.0/PKG-INFO
```

### Comparing `gyver_tests-0.2.2/gyver/tests/config/mocker.py` & `gyver_tests-1.0.0/gyver/tests/config/mocker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 from contextlib import contextmanager
-from typing import Any, Callable, Sequence
+from typing import Any, Callable, Mapping, Optional, Sequence, TypeVar
 
-from gyver.config.provider import ConfigLoader, ProviderConfig, ProviderT
+from gyver.config import AdapterConfigFactory
 
 from .registry import config_map
 
+T = TypeVar("T")
+
 
 class ConfigMocker:
     """
     ConfigMocker is a context manager for mocking provider configurations.
     It allows to mock and use registered providers in a controlled environment
     and revert them to their original behavior when the context is exited."""
 
     def __init__(
         self,
-        *custom_factories: tuple[type[ProviderT], Callable[[], ProviderT]],
+        *custom_factories: tuple[type[T], Callable[[], T]],
     ) -> None:
         """
         :param custom_factories: a list of custom factories, that will override
                                 existing factories with the same config class
         """
-        self.factories: dict[
-            type[ProviderConfig], Callable[[], ProviderConfig]
-        ] = config_map | dict(custom_factories)
-        self._resolved: dict[type[ProviderConfig], ProviderConfig] = {}
+        self.factories: dict[type, Callable[[], Any]] = config_map | dict(
+            custom_factories
+        )
+        self._resolved: dict[type, Any] = {}
 
-    def resolve(self, config_class: type[ProviderConfig]) -> None:
+    def resolve(self, config_class: type) -> None:
         """
         Resolve an instance of a config class using its registered factory
         """
         self._resolved[config_class] = self.factories[config_class]()
 
-    def resolve_all(self, only: Sequence[type[ProviderConfig]] = ()):
+    def resolve_all(self, only: Sequence[type] = ()):
         """
         Resolve all config classes, or the classes
         passed as the `only` argument
         :param only: a list of classes to resolve, the others will be ignored
         """
         to_resolve = self.factories
         if only:
@@ -51,38 +53,38 @@
 
     def unresolve(self):
         """
         Unresolve all config classes
         """
         self._resolved.clear()
 
-    def register(self, config_class: type[ProviderT], factory: Callable[[], ProviderT]):
+    def register(self, config_class: type[T], factory: Callable[[], T]):
         """
         Register a new factory for a config class
         :param config_class: the config class to register the factory for
         :param factory: the factory to use when resolving the config class
         """
         self.factories[config_class] = factory
 
-    def get(self, config_class: type[ProviderT]) -> ProviderT:
+    def get(self, config_class: type[T]) -> T:
         """
         Get an instance of the config class, resolving it if necessary
         :param config_class: the config class to get the instance of
         :returns: an instance of the config class
         """
         if config_class not in self.factories:
             raise ValueError(f"No factory registered for {config_class}")
         try:
             return self._resolved[config_class]  # type: ignore
         except KeyError:
             self.resolve(config_class)
             return self._resolved[config_class]  # type: ignore
 
     @contextmanager
-    def mock(self, only: Sequence[type[ProviderConfig]] = ()):
+    def mock(self, only: Sequence[type] = ()):
         """A context manager to mock the specified configurations
 
         This context manager mocks the specified configuration classes,
         so that they return the registered instances when used.
         The mocked classes are returned to their original state
         when the context manager exits.
 
@@ -98,37 +100,41 @@
         for config_class, instance in self._resolved.items():
             config_class.__new__ = make_custom_method(instance)
             config_class.__init__ = custom_init
 
         get = self.get
 
         def _mocked_load(
-            self: ConfigLoader,
-            model_cls: type[ProviderConfig],
-            **presets: Any,
+            self,
+            model_cls: type,
+            __prefix__: str = "",
+            *,
+            presets: Optional[Mapping[str, Any]] = None,
+            **defaults: Any,
         ):
-            del self, presets
+            del self, presets, defaults
             return get(model_cls)
 
-        original_load, ConfigLoader.load = ConfigLoader.load, _mocked_load
+        original_load, AdapterConfigFactory.load = (
+            AdapterConfigFactory.load,
+            _mocked_load,
+        )
         yield
-        ConfigLoader.load = original_load
+        AdapterConfigFactory.load = original_load
         for config_class, (new, init) in classmethods_map.items():
             config_class.__new__ = new
             config_class.__init__ = init
 
-    def __getitem__(self, config_class: type[ProviderT]) -> ProviderT:
+    def __getitem__(self, config_class: type[T]) -> T:
         try:
             return self.get(config_class)
         except ValueError as e:
             raise KeyError(f"{config_class.__name__} not found") from e
 
-    def __setitem__(
-        self, config_class: type[ProviderT], factory: Callable[[], ProviderT]
-    ):
+    def __setitem__(self, config_class: type[T], factory: Callable[[], T]):
         self.register(config_class, factory)
 
 
 def make_custom_method(return_value: Any):
     """
     Create a custom method that returns the given return_value.
     :param return_value: The value to be returned by the custom method.
```

### Comparing `gyver_tests-0.2.2/gyver/tests/config/registry.py` & `gyver_tests-1.0.0/gyver/tests/config/registry.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import contextlib
-from typing import Callable, Mapping, MutableMapping
+from typing import Any, Callable, Mapping, MutableMapping
 
 from cryptography.fernet import Fernet
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import serialization
 from cryptography.hazmat.primitives.asymmetric import rsa
-
-from gyver.config.provider import ProviderConfig
 from gyver.crypto.config import CryptoConfig
 from gyver.crypto.rsa import RSACryptoConfig
 
 
 def default_crypto_config():
     return CryptoConfig(secret=Fernet.generate_key().decode(), spares=[])
 
@@ -29,27 +27,22 @@
         public_key=public_key.public_bytes(
             encoding=serialization.Encoding.PEM,
             format=serialization.PublicFormat.SubjectPublicKeyInfo,
         ).decode(),
     )
 
 
-_config_map: MutableMapping[type[ProviderConfig], Callable[[], ProviderConfig]] = {
+_config_map: MutableMapping[type, Callable[[], Any]] = {
     CryptoConfig: default_crypto_config,
     RSACryptoConfig: default_rsa_config,
 }
 
 with contextlib.suppress(ImportError):
-    from gyver.boto.storage import StorageConfig
     from gyver.database import DatabaseConfig
     from gyver.database.typedef import Driver
 
     def default_database_config():
         return DatabaseConfig(driver=Driver.SQLITE, host="/:memory")
 
-    def default_storage_config():
-        return StorageConfig(bucket_name="test")
-
     _config_map[DatabaseConfig] = default_database_config
-    _config_map[StorageConfig] = default_storage_config
 
-config_map: Mapping[type[ProviderConfig], Callable[[], ProviderConfig]] = _config_map
+config_map: Mapping[type, Callable[[], Any]] = _config_map
```

### Comparing `gyver_tests-0.2.2/gyver/tests/http/exc.py` & `gyver_tests-1.0.0/gyver/tests/http/exc.py`

 * *Files identical despite different names*

### Comparing `gyver_tests-0.2.2/gyver/tests/http/helpers.py` & `gyver_tests-1.0.0/gyver/tests/http/helpers.py`

 * *Files identical despite different names*

### Comparing `gyver_tests-0.2.2/gyver/tests/http/mocker.py` & `gyver_tests-1.0.0/gyver/tests/http/mocker.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 from functools import wraps
 from http import HTTPStatus
 from unittest.mock import Mock
 
 from aiohttp import ClientSession
 from aiohttp.client import ClientResponse
 from aiohttp.helpers import TimerNoop
-from multidict import CIMultiDict, CIMultiDictProxy
-
 from gyver.utils import json
+from multidict import CIMultiDict, CIMultiDictProxy
 
 from . import exc, helpers, typedef
 
 METHODS = typing.Literal[
     "GET",
     "POST",
     "PUT",
```

### Comparing `gyver_tests-0.2.2/gyver/tests/http/mocker.pyi` & `gyver_tests-1.0.0/gyver/tests/http/mocker.pyi`

 * *Files identical despite different names*

### Comparing `gyver_tests-0.2.2/gyver/tests/http/plugin.py` & `gyver_tests-1.0.0/gyver/tests/http/plugin.py`

 * *Files identical despite different names*

### Comparing `gyver_tests-0.2.2/gyver/tests/http/typedef.py` & `gyver_tests-1.0.0/gyver/tests/http/typedef.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import typing
 from unittest.mock import Mock
 
 import yarl
 from aiohttp.base_protocol import BaseProtocol
 from aiohttp.streams import StreamReader
-
 from gyver.url import URL, Query
 
 
 class FrozenURL:
     def __init__(
         self,
         url: str,
```

### Comparing `gyver_tests-0.2.2/pyproject.toml` & `gyver_tests-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "gyver-tests"
-version = "0.2.2"
+version = "1.0.0"
 description = ""
 authors = ["Gustavo Correa <self.gustavocorrea@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gyver/tests" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-gyver = "^1.0.0"
+gyver = "^2.0.0"
 pytest = "^7.2.1"
 faker = "^16.6.1"
 
 
 [tool.poetry.group.http.dependencies]
 aiohttp = "^3.8.3"
```

### Comparing `gyver_tests-0.2.2/PKG-INFO` & `gyver_tests-1.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: gyver-tests
-Version: 0.2.2
+Version: 1.0.0
 Summary: 
 Author: Gustavo Correa
 Author-email: self.gustavocorrea@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: faker (>=16.6.1,<17.0.0)
-Requires-Dist: gyver (>=1.0.0,<2.0.0)
+Requires-Dist: gyver (>=2.0.0,<3.0.0)
 Requires-Dist: pytest (>=7.2.1,<8.0.0)
 Description-Content-Type: text/markdown
```


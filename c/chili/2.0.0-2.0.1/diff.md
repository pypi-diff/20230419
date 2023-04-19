# Comparing `tmp/chili-2.0.0.tar.gz` & `tmp/chili-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chili-2.0.0.tar", max compression
+gzip compressed data, was "chili-2.0.1.tar", max compression
```

## Comparing `chili-2.0.0.tar` & `chili-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1085 2023-04-18 05:11:12.568292 chili-2.0.0/LICENSE
--rw-r--r--   0        0        0    11664 2023-04-18 05:11:12.568292 chili-2.0.0/README.md
--rw-r--r--   0        0        0      614 2023-04-18 05:11:12.568292 chili-2.0.0/chili/__init__.py
--rw-r--r--   0        0        0       22 2023-04-18 05:11:12.568292 chili-2.0.0/chili/__version__.py
--rw-r--r--   0        0        0    16042 2023-04-18 05:11:12.568292 chili-2.0.0/chili/decoder.py
--rw-r--r--   0        0        0    13956 2023-04-18 05:11:12.568292 chili-2.0.0/chili/encoder.py
--rw-r--r--   0        0        0      411 2023-04-18 05:11:12.568292 chili-2.0.0/chili/error.py
--rw-r--r--   0        0        0     5741 2023-04-18 05:11:12.568292 chili-2.0.0/chili/iso_datetime.py
--rw-r--r--   0        0        0     1093 2023-04-18 05:11:12.568292 chili-2.0.0/chili/json_support.py
--rw-r--r--   0        0        0     3155 2023-04-18 05:11:12.568292 chili-2.0.0/chili/mapper.py
--rw-r--r--   0        0        0        0 2023-04-18 05:11:12.568292 chili-2.0.0/chili/py.typed
--rw-r--r--   0        0        0     1513 2023-04-18 05:11:12.568292 chili-2.0.0/chili/serializer.py
--rw-r--r--   0        0        0      260 2023-04-18 05:11:12.568292 chili-2.0.0/chili/state.py
--rw-r--r--   0        0        0     6043 2023-04-18 05:11:12.568292 chili-2.0.0/chili/typing.py
--rw-r--r--   0        0        0     1228 2023-04-18 05:11:12.568292 chili-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    13059 1970-01-01 00:00:00.000000 chili-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-19 16:12:17.796775 chili-2.0.1/LICENSE
+-rw-r--r--   0        0        0    12227 2023-04-19 16:12:17.796775 chili-2.0.1/README.md
+-rw-r--r--   0        0        0      614 2023-04-19 16:12:17.796775 chili-2.0.1/chili/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-19 16:12:17.800775 chili-2.0.1/chili/__version__.py
+-rw-r--r--   0        0        0    16042 2023-04-19 16:12:17.800775 chili-2.0.1/chili/decoder.py
+-rw-r--r--   0        0        0    13956 2023-04-19 16:12:17.800775 chili-2.0.1/chili/encoder.py
+-rw-r--r--   0        0        0      411 2023-04-19 16:12:17.800775 chili-2.0.1/chili/error.py
+-rw-r--r--   0        0        0     5741 2023-04-19 16:12:17.800775 chili-2.0.1/chili/iso_datetime.py
+-rw-r--r--   0        0        0     1093 2023-04-19 16:12:17.800775 chili-2.0.1/chili/json_support.py
+-rw-r--r--   0        0        0     3155 2023-04-19 16:12:17.800775 chili-2.0.1/chili/mapper.py
+-rw-r--r--   0        0        0        0 2023-04-19 16:12:17.800775 chili-2.0.1/chili/py.typed
+-rw-r--r--   0        0        0     1513 2023-04-19 16:12:17.800775 chili-2.0.1/chili/serializer.py
+-rw-r--r--   0        0        0      260 2023-04-19 16:12:17.800775 chili-2.0.1/chili/state.py
+-rw-r--r--   0        0        0     6361 2023-04-19 16:12:17.800775 chili-2.0.1/chili/typing.py
+-rw-r--r--   0        0        0     1228 2023-04-19 16:12:17.800775 chili-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    13622 1970-01-01 00:00:00.000000 chili-2.0.1/PKG-INFO
```

### Comparing `chili-2.0.0/LICENSE` & `chili-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chili-2.0.0/README.md` & `chili-2.0.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 Chili is an extensible library which provides a simple and efficient way to encode and decode complex Python objects to and from their dictionary representation.
 
 It offers complete coverage for the `typing` package; including generics, and supports custom types, allowing you to extend the library to handle your specific needs. 
 
 With support for nested data structures, default values, forward references, and data mapping and transformation, Chili is designed to be both easy to use and powerful enough to handle complex data structures.
 
+> Note: Chili is not a validation library, although it ensures the type integrity. 
+
 # Installation
 
 To install the library, simply use pip:
 
 ```shell
 pip install chili
 ```
@@ -19,14 +21,18 @@
 poetry add chili
 ```
 
 # Usage
 
 The library provides three main classes for encoding and decoding objects, `chili.Encoder` and `chili.Decoder`, and `chili.Serializer`, which combines both functionalities.
 
+Convinient functions are also provided for encoding and decoding objects, `chili.encode` and `chili.decode`.
+
+Additionally, library by default supports json serialization and deserialization, so you can use `chili.JsonDecoder`, and `chili.JsonDecoder`, and `chili.JsonSerializer` or its functional replacement `chili.json_encode` and `chili.json_decode` to serialize and deserialize objects to and from json.
+
 ## Defining encodable/decodable properties
 To define the properties of a class that should be encoded and decoded, you need to define them with type annotations. 
 The `@encodable`, `@decodable`, or `@serializable` decorator should also be used to mark the class as encodable/decodable or serializable.
 
 ```python
 from chili import encodable
 
@@ -106,30 +112,30 @@
 
 ## Custom Type Encoders
 You can also specify custom type encoders by defining a class that implements the `chili.TypeEncoder` protocol and passing it as a dictionary to the `encoders` argument of the Encoder constructor.
 
 ```python
 from chili import Encoder, TypeEncoder
 
-class MyCustomEncoder(TypeEncoder[MyCustomType, str]):
+class MyCustomEncoder(TypeEncoder):
     def encode(self, value: MyCustomType) -> str:
         return value.encode()
 
     
 type_encoders = {MyCustomType: MyCustomEncoder()}
 encoder = Encoder[Pet](encoders=type_encoders)
 ```
 
 ## Custom Type Decoders
 You can also specify custom type decoders by defining a class that implements the `chili.TypeDecoder` protocol and passing it as a dictionary to the `decoders` argument of the Decoder constructor.
 
 ```python
 from chili import Decoder, TypeDecoder
 
-class MyCustomDecoder(TypeDecoder[str, MyCustomType]):
+class MyCustomDecoder(TypeDecoder):
     def decode(self, value: str) -> MyCustomType:
         return MyCustomType.decode(value)
 
 type_decoders = {MyCustomType: MyCustomDecoder()}
 decoder = Decoder[Pet](decoders=type_decoders)
 ```
 
@@ -192,14 +198,16 @@
 
 ```json
 {"name": "Max", "age": 3, "breed": "Golden Retriever"}
 ```
 
 The `decoded` value will be an instance of a Pet object.
 
+> Functional interface is also available through the `chili.json_encode`, `chili.json_decode` functions.
+
 ## Mapping
 
 Mapping allows you to remap keys, apply functions to the values, and even change the structure of the input dictionary. This is particularly useful when you need to convert data from one format to another, such as when interacting with different APIs or data sources that use different naming conventions.
 
 ### Simple mapping
 Here's an example of how to use the `chili.Mapper` class from the library with a Pet class:
```

### Comparing `chili-2.0.0/chili/__init__.py` & `chili-2.0.1/chili/__init__.py`

 * *Files identical despite different names*

### Comparing `chili-2.0.0/chili/decoder.py` & `chili-2.0.1/chili/decoder.py`

 * *Files identical despite different names*

### Comparing `chili-2.0.0/chili/encoder.py` & `chili-2.0.1/chili/encoder.py`

 * *Files identical despite different names*

### Comparing `chili-2.0.0/chili/iso_datetime.py` & `chili-2.0.1/chili/iso_datetime.py`

 * *Files identical despite different names*

### Comparing `chili-2.0.0/chili/json_support.py` & `chili-2.0.1/chili/json_support.py`

 * *Files identical despite different names*

### Comparing `chili-2.0.0/chili/mapper.py` & `chili-2.0.1/chili/mapper.py`

 * *Files identical despite different names*

### Comparing `chili-2.0.0/chili/serializer.py` & `chili-2.0.1/chili/serializer.py`

 * *Files identical despite different names*

### Comparing `chili-2.0.0/chili/typing.py` & `chili-2.0.1/chili/typing.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import sys
 import typing
 from dataclasses import Field, is_dataclass, MISSING
 from enum import Enum
 from inspect import isclass as is_class
 from typing import Any, Dict, List, Optional, Type, Union, ClassVar, NewType, Callable
 
+from chili.error import SerialisationError
+
 AnnotatedTypeNames = {"AnnotatedMeta", "_AnnotatedAlias"}
 _GenericAlias = getattr(typing, "_GenericAlias")
 _PROPERTIES = "__typed_properties__"
 _ENCODABLE = "__encodable__"
 _DECODABLE = "__decodable__"
 UNDEFINED = object()
 
@@ -113,19 +115,27 @@
     if type_args:
         mapped_args = tuple([type_map[arg] for arg in type_args])
         return _GenericAlias(origin_type, mapped_args)
 
     return type_name
 
 
-def resolve_forward_reference(module: Any, ref: typing.ForwardRef) -> Any:
-    name = ref.__forward_arg__
+def resolve_forward_reference(module: Any, ref: Union[typing.ForwardRef, str]) -> Any:
+    if isinstance(ref, typing.ForwardRef):
+        name = ref.__forward_arg__
+    else:
+        name = ref
     if name in sys.modules[module].__dict__:
         return sys.modules[module].__dict__[name]
 
+    if name in sys.modules["builtins"].__dict__:
+        return sys.modules["builtins"].__dict__[name]
+
+
+
     return None
 
 
 class Property:
     __slots__ = ("name", "type", "_default_value", "_default_factory")
 
     def __init__(
@@ -153,15 +163,18 @@
 TypeSchema = NewType("TypeSchema", Dict[str, Property])
 
 
 _default_factories = (list, dict, tuple, set, bytes, bytearray, frozenset)
 
 
 def create_schema(cls: Type) -> TypeSchema:
-    properties = cls.__dict__.get("__annotations__", {})
+    try:
+        properties = typing.get_type_hints(cls)
+    except NameError as e:
+        raise SerialisationError.invalid_type from e
 
     schema = TypeSchema({})
     base_classes = [base_class for base_class in cls.__mro__[1:-1] if hasattr(base_class, _PROPERTIES)]
     for base_class in base_classes:
         schema = {**getattr(base_class, _PROPERTIES), **schema}  # type: ignore
 
     attributes = {name: value for name, value in cls.__dict__.items() if not name.startswith("__")}
```

### Comparing `chili-2.0.0/pyproject.toml` & `chili-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 documentation = "https://github.com/kodemore/chili"
 homepage = "https://github.com/kodemore/chili"
 keywords = ["serialise", "deserialise", "encode", "decode", "object", "class"]
 license = "MIT"
 name = "chili"
 readme = "README.md"
 repository = "https://github.com/kodemore/chili"
-version = "2.0.0"
+version = "2.0.1"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typing-extensions = "^4.2"
 gaffe = "0.2.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `chili-2.0.0/PKG-INFO` & `chili-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chili
-Version: 2.0.0
+Version: 2.0.1
 Summary: Chili is serialisation library. It can serialise/deserialise almost any object.
 Home-page: https://github.com/kodemore/chili
 License: MIT
 Keywords: serialise,deserialise,encode,decode,object,class
 Author: Dawid Kraczkowski
 Author-email: dawid.kraczkowski@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -35,14 +35,16 @@
 
 Chili is an extensible library which provides a simple and efficient way to encode and decode complex Python objects to and from their dictionary representation.
 
 It offers complete coverage for the `typing` package; including generics, and supports custom types, allowing you to extend the library to handle your specific needs. 
 
 With support for nested data structures, default values, forward references, and data mapping and transformation, Chili is designed to be both easy to use and powerful enough to handle complex data structures.
 
+> Note: Chili is not a validation library, although it ensures the type integrity. 
+
 # Installation
 
 To install the library, simply use pip:
 
 ```shell
 pip install chili
 ```
@@ -51,14 +53,18 @@
 poetry add chili
 ```
 
 # Usage
 
 The library provides three main classes for encoding and decoding objects, `chili.Encoder` and `chili.Decoder`, and `chili.Serializer`, which combines both functionalities.
 
+Convinient functions are also provided for encoding and decoding objects, `chili.encode` and `chili.decode`.
+
+Additionally, library by default supports json serialization and deserialization, so you can use `chili.JsonDecoder`, and `chili.JsonDecoder`, and `chili.JsonSerializer` or its functional replacement `chili.json_encode` and `chili.json_decode` to serialize and deserialize objects to and from json.
+
 ## Defining encodable/decodable properties
 To define the properties of a class that should be encoded and decoded, you need to define them with type annotations. 
 The `@encodable`, `@decodable`, or `@serializable` decorator should also be used to mark the class as encodable/decodable or serializable.
 
 ```python
 from chili import encodable
 
@@ -138,30 +144,30 @@
 
 ## Custom Type Encoders
 You can also specify custom type encoders by defining a class that implements the `chili.TypeEncoder` protocol and passing it as a dictionary to the `encoders` argument of the Encoder constructor.
 
 ```python
 from chili import Encoder, TypeEncoder
 
-class MyCustomEncoder(TypeEncoder[MyCustomType, str]):
+class MyCustomEncoder(TypeEncoder):
     def encode(self, value: MyCustomType) -> str:
         return value.encode()
 
     
 type_encoders = {MyCustomType: MyCustomEncoder()}
 encoder = Encoder[Pet](encoders=type_encoders)
 ```
 
 ## Custom Type Decoders
 You can also specify custom type decoders by defining a class that implements the `chili.TypeDecoder` protocol and passing it as a dictionary to the `decoders` argument of the Decoder constructor.
 
 ```python
 from chili import Decoder, TypeDecoder
 
-class MyCustomDecoder(TypeDecoder[str, MyCustomType]):
+class MyCustomDecoder(TypeDecoder):
     def decode(self, value: str) -> MyCustomType:
         return MyCustomType.decode(value)
 
 type_decoders = {MyCustomType: MyCustomDecoder()}
 decoder = Decoder[Pet](decoders=type_decoders)
 ```
 
@@ -224,14 +230,16 @@
 
 ```json
 {"name": "Max", "age": 3, "breed": "Golden Retriever"}
 ```
 
 The `decoded` value will be an instance of a Pet object.
 
+> Functional interface is also available through the `chili.json_encode`, `chili.json_decode` functions.
+
 ## Mapping
 
 Mapping allows you to remap keys, apply functions to the values, and even change the structure of the input dictionary. This is particularly useful when you need to convert data from one format to another, such as when interacting with different APIs or data sources that use different naming conventions.
 
 ### Simple mapping
 Here's an example of how to use the `chili.Mapper` class from the library with a Pet class:
```


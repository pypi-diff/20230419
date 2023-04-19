# Comparing `tmp/AssertionLib-3.2.1.tar.gz` & `tmp/AssertionLib-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AssertionLib-3.2.1.tar", last modified: Tue Oct 12 10:42:08 2021, max compression
+gzip compressed data, was "AssertionLib-3.2.2.tar", last modified: Wed Apr 19 17:15:35 2023, max compression
```

## Comparing `AssertionLib-3.2.1.tar` & `AssertionLib-3.2.2.tar`

### file list

```diff
@@ -1,22 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 10:42:08.278290 AssertionLib-3.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 10:42:08.278290 AssertionLib-3.2.1/AssertionLib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6698 2021-10-12 10:42:08.000000 AssertionLib-3.2.1/AssertionLib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      454 2021-10-12 10:42:08.000000 AssertionLib-3.2.1/AssertionLib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-12 10:42:08.000000 AssertionLib-3.2.1/AssertionLib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-12 10:42:08.000000 AssertionLib-3.2.1/AssertionLib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      328 2021-10-12 10:42:08.000000 AssertionLib-3.2.1/AssertionLib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-10-12 10:42:08.000000 AssertionLib-3.2.1/AssertionLib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-10-12 10:41:26.000000 AssertionLib-3.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-12 10:41:26.000000 AssertionLib-3.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6698 2021-10-12 10:42:08.278290 AssertionLib-3.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5337 2021-10-12 10:41:26.000000 AssertionLib-3.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-12 10:42:08.278290 AssertionLib-3.2.1/assertionlib/
--rw-r--r--   0 runner    (1001) docker     (121)      639 2021-10-12 10:41:26.000000 AssertionLib-3.2.1/assertionlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-10-12 10:41:26.000000 AssertionLib-3.2.1/assertionlib/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4614 2021-10-12 10:41:26.000000 AssertionLib-3.2.1/assertionlib/assertion_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    16625 2021-10-12 10:41:26.000000 AssertionLib-3.2.1/assertionlib/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (121)    15021 2021-10-12 10:41:26.000000 AssertionLib-3.2.1/assertionlib/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    25132 2021-10-12 10:41:26.000000 AssertionLib-3.2.1/assertionlib/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)    19164 2021-10-12 10:41:26.000000 AssertionLib-3.2.1/assertionlib/ndrepr.py
--rw-r--r--   0 runner    (1001) docker     (121)      577 2021-10-12 10:42:08.278290 AssertionLib-3.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3025 2021-10-12 10:41:26.000000 AssertionLib-3.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:15:35.616062 AssertionLib-3.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:15:35.612062 AssertionLib-3.2.2/AssertionLib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-19 17:15:35.000000 AssertionLib-3.2.2/AssertionLib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-19 17:15:35.000000 AssertionLib-3.2.2/AssertionLib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:15:35.000000 AssertionLib-3.2.2/AssertionLib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 17:15:35.000000 AssertionLib-3.2.2/AssertionLib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-19 17:15:35.000000 AssertionLib-3.2.2/AssertionLib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 17:15:35.000000 AssertionLib-3.2.2/AssertionLib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-04-19 17:15:35.616062 AssertionLib-3.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:15:35.616062 AssertionLib-3.2.2/assertionlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/assertionlib/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/assertionlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/assertionlib/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/assertionlib/assertion_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16614 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/assertionlib/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15087 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/assertionlib/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25132 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/assertionlib/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27489 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/assertionlib/manager.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19175 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/assertionlib/ndrepr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/assertionlib/protocol.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/assertionlib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-19 17:15:35.616062 AssertionLib-3.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 17:15:35.616062 AssertionLib-3.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/tests/test_dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9866 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/tests/test_manager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1814 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/tests/test_manager_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11203 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/tests/test_manager_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/tests/test_manager_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/tests/test_ndrepr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-19 17:15:13.000000 AssertionLib-3.2.2/tests/test_sphinx.py
```

### Comparing `AssertionLib-3.2.1/AssertionLib.egg-info/PKG-INFO` & `AssertionLib-3.2.2/AssertionLib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: AssertionLib
-Version: 3.2.1
+Version: 3.2.2
 Summary: A package for performing assertions and providing informative exception messages.
 Home-page: https://github.com/nlesc-nano/AssertionLib
 Author: ['B. F. van Beek']
 Author-email: b.f.van.beek@vu.nl
 License: Apache Software License
-Keywords: assertion,assertions,assertion-library,testing,unit-testing,python-3,python-3-6,python-3-7,python-3-8,python-3-9,python-3-10
-Platform: UNKNOWN
+Keywords: assertion,assertions,assertion-library,testing,unit-testing,python-3,python-3-6,python-3-7,python-3-8,python-3-9,python-3-10,python-3-11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: test_no_optional
-Provides-Extra: build
 License-File: LICENSE.md
 
 .. image:: https://readthedocs.org/projects/assertionlib/badge/?version=latest
     :target: https://assertionlib.readthedocs.io/en/latest/
 .. image:: https://badge.fury.io/py/AssertionLib.svg
     :target: https://badge.fury.io/py/AssertionLib
 .. image:: https://github.com/nlesc-nano/AssertionLib/workflows/Python%20package/badge.svg
@@ -48,19 +47,22 @@
     :target: https://docs.python.org/3.6/
 .. image:: https://img.shields.io/badge/python-3.7-blue.svg
     :target: https://docs.python.org/3.7/
 .. image:: https://img.shields.io/badge/python-3.8-blue.svg
     :target: https://docs.python.org/3.8/
 .. image:: https://img.shields.io/badge/python-3.9-blue.svg
     :target: https://docs.python.org/3.9/
-
-
-##################
-AssertionLib 3.2.1
-##################
+.. image:: https://img.shields.io/badge/python-3.10-blue.svg
+    :target: https://docs.python.org/3.10/
+.. image:: https://img.shields.io/badge/python-3.11-blue.svg
+    :target: https://docs.python.org/3.11/
+
+############
+AssertionLib
+############
 A package for performing assertions and providing informative exception messages.
 
 
 Installation
 ************
 * PyPi: ``pip install AssertionLib``
 * GitHub: ``pip install git+https://github.com/nlesc-nano/AssertionLib``
@@ -208,9 +210,7 @@
 
     output: bool = False
     a: int = 5
 
 .. _documentation: https://assertionlib.readthedocs.io/en/latest/3_assertionmanager.html
 
 
-
-
```

### Comparing `AssertionLib-3.2.1/LICENSE.md` & `AssertionLib-3.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `AssertionLib-3.2.1/PKG-INFO` & `AssertionLib-3.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 Metadata-Version: 2.1
 Name: AssertionLib
-Version: 3.2.1
+Version: 3.2.2
 Summary: A package for performing assertions and providing informative exception messages.
 Home-page: https://github.com/nlesc-nano/AssertionLib
 Author: ['B. F. van Beek']
 Author-email: b.f.van.beek@vu.nl
 License: Apache Software License
-Keywords: assertion,assertions,assertion-library,testing,unit-testing,python-3,python-3-6,python-3-7,python-3-8,python-3-9,python-3-10
-Platform: UNKNOWN
+Keywords: assertion,assertions,assertion-library,testing,unit-testing,python-3,python-3-6,python-3-7,python-3-8,python-3-9,python-3-10,python-3-11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: test_no_optional
-Provides-Extra: build
 License-File: LICENSE.md
 
 .. image:: https://readthedocs.org/projects/assertionlib/badge/?version=latest
     :target: https://assertionlib.readthedocs.io/en/latest/
 .. image:: https://badge.fury.io/py/AssertionLib.svg
     :target: https://badge.fury.io/py/AssertionLib
 .. image:: https://github.com/nlesc-nano/AssertionLib/workflows/Python%20package/badge.svg
@@ -48,19 +47,22 @@
     :target: https://docs.python.org/3.6/
 .. image:: https://img.shields.io/badge/python-3.7-blue.svg
     :target: https://docs.python.org/3.7/
 .. image:: https://img.shields.io/badge/python-3.8-blue.svg
     :target: https://docs.python.org/3.8/
 .. image:: https://img.shields.io/badge/python-3.9-blue.svg
     :target: https://docs.python.org/3.9/
-
-
-##################
-AssertionLib 3.2.1
-##################
+.. image:: https://img.shields.io/badge/python-3.10-blue.svg
+    :target: https://docs.python.org/3.10/
+.. image:: https://img.shields.io/badge/python-3.11-blue.svg
+    :target: https://docs.python.org/3.11/
+
+############
+AssertionLib
+############
 A package for performing assertions and providing informative exception messages.
 
 
 Installation
 ************
 * PyPi: ``pip install AssertionLib``
 * GitHub: ``pip install git+https://github.com/nlesc-nano/AssertionLib``
@@ -208,9 +210,7 @@
 
     output: bool = False
     a: int = 5
 
 .. _documentation: https://assertionlib.readthedocs.io/en/latest/3_assertionmanager.html
 
 
-
-
```

### Comparing `AssertionLib-3.2.1/README.rst` & `AssertionLib-3.2.2/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -15,19 +15,22 @@
     :target: https://docs.python.org/3.6/
 .. image:: https://img.shields.io/badge/python-3.7-blue.svg
     :target: https://docs.python.org/3.7/
 .. image:: https://img.shields.io/badge/python-3.8-blue.svg
     :target: https://docs.python.org/3.8/
 .. image:: https://img.shields.io/badge/python-3.9-blue.svg
     :target: https://docs.python.org/3.9/
+.. image:: https://img.shields.io/badge/python-3.10-blue.svg
+    :target: https://docs.python.org/3.10/
+.. image:: https://img.shields.io/badge/python-3.11-blue.svg
+    :target: https://docs.python.org/3.11/
 
-
-##################
-AssertionLib 3.2.1
-##################
+############
+AssertionLib
+############
 A package for performing assertions and providing informative exception messages.
 
 
 Installation
 ************
 * PyPi: ``pip install AssertionLib``
 * GitHub: ``pip install git+https://github.com/nlesc-nano/AssertionLib``
```

### Comparing `AssertionLib-3.2.1/assertionlib/assertion_functions.py` & `AssertionLib-3.2.2/assertionlib/assertion_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,18 +20,20 @@
 .. autofunction:: isdisjoint
 .. autofunction:: issuperset
 .. autofunction:: issubset
 .. autofunction:: function_eq
 
 """
 
+import warnings
 import dis
 from types import FunctionType
 from itertools import zip_longest
 from typing import (
+    Any,
     Sized,
     Callable,
     TypeVar,
     Iterable,
     Union,
     Tuple,
     Hashable,
@@ -60,22 +62,22 @@
 @to_positional
 def str_eq(a: T, b: str, *, str_converter: Callable[[T], str] = repr) -> bool:
     """Check if the string-representation of **a** is equivalent to **b**: :code:`repr(a) == b`."""
     return str_converter(a) == b
 
 
 @to_positional
-def shape_eq(a: ndarray, b: Union[ndarray, Tuple[int, ...]]) -> bool:
+def shape_eq(a: "ndarray[Any, Any]", b: Union["ndarray[Any, Any]", Tuple[int, ...]]) -> bool:
     """Check if the shapes of **a** and **b** are equivalent: :code:`a.shape == getattr(b, 'shape', b)`.
 
     **b** should be either an object with the ``shape`` attribute (*e.g.* a NumPy array)
     or a :class:`tuple` representing a valid array shape.
 
     """  # noqa: E501
-    return a.shape == getattr(b, 'shape', b)  # type: ignore
+    return a.shape == getattr(b, 'shape', b)
 
 
 @to_positional
 def isdisjoint(a: Iterable[Hashable], b: Iterable[Hashable]) -> bool:
     """Check if **a** has no elements in **b**."""
     try:
         return a.isdisjoint(b)  # type: ignore
@@ -132,14 +134,19 @@
 def function_eq(func1: FunctionType, func2: FunctionType) -> bool:
     """Check if two functions are equivalent by checking if their :attr:`__code__` is identical.
 
     **func1** and **func2** should be instances of :data:`~types.FunctionType`
     or any other object with access to the :attr:`__code__` attribute.
 
     """
+    warnings.warn(
+        "`function_eq` is deprecated and will be removed in the future",
+        DeprecationWarning, stacklevel=2,
+    )
+
     code1 = None
     try:
         code1 = func1.__code__
         code2 = func2.__code__
     except AttributeError as ex:
         name, obj = ('func1', func1) if code1 is None else ('func2', func2)
         raise TypeError(f"{name!r} expected a function or object with the '__code__' attribute; "
```

### Comparing `AssertionLib-3.2.1/assertionlib/dataclass.py` & `AssertionLib-3.2.2/assertionlib/dataclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     Implementation based on :func:`reprlib.recursive_repr`.
 
     """
     def decorating_function(user_function: FT) -> FT:
         running: Set[Tuple[int, int]] = set()
 
         @wraps(user_function)
-        def wrapper(self, *args: Any, **kwargs: Any) -> Any:
+        def wrapper(self: Any, *args: Any, **kwargs: Any) -> Any:
             key = id(self), get_ident()
             if key in running:
                 return fallback(self, *args, **kwargs)
 
             running.add(key)
             try:
                 result = user_function(self, *args, **kwargs)
@@ -406,15 +406,15 @@
 
         See Also
         --------
         :meth:`AbstractDataClass.as_dict`
             Construct a dictionary from this instance with all non-private instance variables.
 
         """
-        return cls(**dct)  # type: ignore
+        return cls(**dct)
 
     @classmethod
     def inherit_annotations(cls) -> Callable[[FT], FT]:
         """A decorator for inheriting annotations and docstrings.
 
         Can be applied to methods of :class:`AbstractDataClass` subclasses to automatically
         inherit the docstring and annotations of identical-named functions of its superclass.
```

### Comparing `AssertionLib-3.2.1/assertionlib/functions.py` & `AssertionLib-3.2.2/assertionlib/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     prm_list = _to_positional(prm_dict.values())
     func.__signature__ = Signature(  # type: ignore
         parameters=prm_list, return_annotation=sgn.return_annotation
     )
     return func
 
 
-def bind_callable(class_type: Union[type, Any], func: Callable,
+def bind_callable(class_type: Union[type, Any], func: Callable[..., Any],
                   name: Optional[str] = None, warn: bool = True) -> None:
     """Take a callable and use it to create a new assertion method for **class_type**.
 
     The created callable will have the same signature as **func** except for one additional
     keyword argument by the name of ``func`` (default value: :data:`False`).
     Setting this keyword argument to :data:`True` will invert the output of the assertion,
     *i.e.* it changes ``assert func(...)`` into ``assert not func(...)``.
@@ -180,15 +180,15 @@
         method = MethodType(function, class_type)  # Create a bound method
         setattr(class_type, function.__name__, method)
 
 
 def create_assertion_func(func: Callable[..., Any]) -> Callable[..., None]:
     """Construct an assertion function from **func**."""
 
-    def wrapper(self, *args: Any,
+    def wrapper(self: Any, *args: Any,
                 invert: bool = False,
                 exception: Optional[Type[Exception]] = None,
                 post_process: Optional[Callable[[Any], Any]] = None,
                 message: Optional[str] = None,
                 **kwargs: Any) -> None:
         __tracebackhide__ = True
 
@@ -246,15 +246,15 @@
 See also
 --------
 {domain}
 {summary}
 """
 
 
-def create_assertion_doc(func: Callable) -> str:
+def create_assertion_doc(func: Callable[..., Any]) -> str:
     r"""Create a new NumPy style assertion docstring from the docstring of **func**.
 
     The summary of **funcs'** docstring, if available, is added to the ``"See also"`` section,
     in addition with an intersphinx-compatible link to **func**.
 
     Examples
     --------
@@ -339,27 +339,30 @@
 
     return BASE_DOCSTRING.format(
         parameters=parameters, name=name, signature=sgn_str, domain=domain, summary=summary
     )
 
 
 #: A dictionary which translates certain __module__ values to an actual valid modules
-MODULE_DICT: Mapping[str, str] = MappingProxyType({
+MODULE_DICT = MappingProxyType({
     'genericpath': 'os.path',
     'posixpath': 'os.path',
     '_operator': 'operator'
 })
 
 
-def _is_builtin_func(func: Callable) -> bool:
+def _is_builtin_func(func: Callable[..., Any]) -> bool:
     """Check if **func** is a builtin function."""
     return isbuiltin(func) and '.' not in getattr(func, '__qualname__', '')
 
 
-def get_sphinx_domain(func: Callable, module_mapping: Mapping[str, str] = MODULE_DICT) -> str:
+def get_sphinx_domain(
+    func: Callable[..., Any],
+    module_mapping: Mapping[str, str] = MODULE_DICT,
+) -> str:
     """Create a Sphinx domain for **func**.
 
     Examples
     --------
     .. code:: python
 
         >>> from collections import OrderedDict
@@ -436,15 +439,15 @@
 #: An immutable mapping of to-be replaced substrings and their replacements.
 README_MAPPING: Mapping[str, str] = MappingProxyType({
     '``': '|',
     '()': ''
 })
 
 
-def load_readme(readme: Union[str, bytes, int, os.PathLike],
+def load_readme(readme: Union[str, bytes, int, "os.PathLike[str]", "os.PathLike[bytes]"],
                 replace: Mapping[str, str] = README_MAPPING,
                 **kwargs: Any) -> str:
     r"""Load and return the content of a readme file located in the same directory as this file.
 
     Equivalent to importing the content of ``../README.rst``.
 
     Parameters
```

### Comparing `AssertionLib-3.2.1/assertionlib/manager.py` & `AssertionLib-3.2.2/assertionlib/manager.py`

 * *Files identical despite different names*

### Comparing `AssertionLib-3.2.1/assertionlib/ndrepr.py` & `AssertionLib-3.2.2/assertionlib/ndrepr.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,17 +75,15 @@
     TYPE_CHECKING,
     KeysView,
     ValuesView,
     ItemsView,
 )
 
 
-from nanoutils import raise_if
-
-from .functions import set_docstring
+from nanoutils import raise_if, set_docstring
 
 if TYPE_CHECKING:
     import numpy as np
     from scm.plams import Molecule, Atom, Bond, Settings
     from numpy import ndarray
     from pandas import DataFrame, Series
     from h5py import Dataset
@@ -363,15 +361,15 @@
             if len(signature) > i:
                 param_accumulate += ', ...'
                 break
             param_accumulate += f', {param}'
 
         return f'{param_accumulate}){ret}'
 
-    def _parse_callable(self, obj: Callable, level: int) -> Tuple[str, str]:
+    def _parse_callable(self, obj: Callable[..., Any], level: int) -> Tuple[str, str]:
         """Create a :class:`str` representation of the name and signature of a callable."""
         # Construct the name of the callable
         name: str = getattr(obj, '__qualname__', obj.__name__)
 
         # Construct the signature
         try:
             _signature = inspect.signature(obj)
@@ -458,15 +456,15 @@
     def repr_Bond(self, obj: Bond, level: int) -> str:  # noqa: N802
         """Create a :class:`str` representation of a |plams.Bond| instance."""
         return f'{obj.__class__.__name__}({obj})'
 
     # NumPy- and Pandas-related methods
 
     @raise_if(NUMPY_EX)
-    def repr_ndarray(self, obj: ndarray, level: int) -> str:
+    def repr_ndarray(self, obj: "ndarray[Any, Any]", level: int) -> str:
         """Create a :class:`str` representation of a :class:`numpy.ndarray` instance."""
         if level <= 0:
             return f'{obj.__class__.__name__}(...)'
 
         kwargs: _FormatOptions = {
             'threshold': self.maxndarray,
             'edgeitems': self.maxndarray // 2,
@@ -506,15 +504,15 @@
         with pd.option_context(*args):
             return builtins.repr(obj)
 
     def repr_Dataset(self, obj: Dataset, level: int) -> str:  # noqa: N802
         """Create a :class:`str` representation of a :class:`h5py.Dataset` instance."""
         return repr(obj)
 
-    def _get_ndformatter(self, obj: ndarray) -> _FormatDict:
+    def _get_ndformatter(self, obj: "ndarray[Any, Any]") -> _FormatDict:
         """Return a value for the **formatter** argument in :func:`numpy.printoptions`."""
         if obj.dtype != float and obj.dtype != int:
             return {}
 
         try:
             max_len = len(str(int(obj.max())))
             min_len = len(str(int(obj.min())))
```

### Comparing `AssertionLib-3.2.1/setup.cfg` & `AssertionLib-3.2.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-description-file = README.rst
+description_file = README.rst
 license_files = LICENSE.md
 
 [aliases]
 test = pytest
 
 [coverage:run]
 branch = True
```

### Comparing `AssertionLib-3.2.1/setup.py` & `AssertionLib-3.2.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,38 +14,30 @@
     exec(f.read(), version)
 
 with open('README.rst', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 # Requirements for building the documentation
 docs_require = [
-    'sphinx>=2.4,<3.1',
+    'sphinx>=2.4',
     'sphinx_rtd_theme'
 ]
 
-# Requirements for building wheels
-build_require = [
-    'twine',
-    'wheel',
-]
-
 tests_require_no_optional = [
     'pytest>=5.4.0',
     'pytest-cov',
-    'pytest-mypy>=0.6.2',
 ]
 
 # Requirements for running tests
 tests_require = [
     'numpy',
     'pandas',
 ]
 tests_require += tests_require_no_optional
 tests_require += docs_require
-tests_require += build_require
 
 setup(
     name='AssertionLib',
     version=version['__version__'],
     description='A package for performing assertions and providing informative exception messages.',
     long_description=f'{readme}\n\n',
     long_description_content_type='text/x-rst',
@@ -66,39 +58,40 @@
         'unit-testing',
         'python-3',
         'python-3-6',
         'python-3-7',
         'python-3-8',
         'python-3-9',
         'python-3-10',
+        'python-3-11',
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Testing',
         'Typing :: Typed',
     ],
     python_requires='>=3.6',
     install_requires=[
-        'Nano-Utils>=0.4.1; python_version<"3.9"',
-        'Nano-Utils>=1.1.2; python_version>="3.9"',
+        'Nano-Utils>=0.4.1; python_version=="3.6"',
+        'Nano-Utils>=2.3.1; python_version>="3.7"',
     ],
     setup_requires=['pytest-runner'] + docs_require,
     tests_require=tests_require,
     extras_require={
         'doc': docs_require,
         'test': tests_require,
         'test_no_optional': tests_require_no_optional,
-        'build': build_require,
     }
 )
```


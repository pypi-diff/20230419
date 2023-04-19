# Comparing `tmp/registtro-1.3.0.tar.gz` & `tmp/registtro-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "registtro-1.3.0.tar", last modified: Sat Jan  7 02:25:29 2023, max compression
+gzip compressed data, was "registtro-1.4.0.tar", last modified: Wed Apr 19 16:28:24 2023, max compression
```

## Comparing `registtro-1.3.0.tar` & `registtro-1.4.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 02:25:29.592619 registtro-1.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 02:25:29.588619 registtro-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 02:25:29.592619 registtro-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-01-07 02:25:11.000000 registtro-1.3.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-07 02:25:11.000000 registtro-1.3.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-01-07 02:25:11.000000 registtro-1.3.0/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-01-07 02:25:11.000000 registtro-1.3.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-01-07 02:25:11.000000 registtro-1.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-07 02:25:11.000000 registtro-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-01-07 02:25:11.000000 registtro-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-01-07 02:25:29.596619 registtro-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-01-07 02:25:11.000000 registtro-1.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 02:25:29.588619 registtro-1.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 02:25:29.592619 registtro-1.3.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 02:25:29.592619 registtro-1.3.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-01-07 02:25:11.000000 registtro-1.3.0/docs/source/_static/registtro.svg
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-01-07 02:25:11.000000 registtro-1.3.0/docs/source/_static/registtro_white.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 02:25:29.592619 registtro-1.3.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-01-07 02:25:11.000000 registtro-1.3.0/docs/source/api/registtro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-01-07 02:25:11.000000 registtro-1.3.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-01-07 02:25:11.000000 registtro-1.3.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 02:25:29.592619 registtro-1.3.0/registtro/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-07 02:25:11.000000 registtro-1.3.0/registtro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-07 02:25:11.000000 registtro-1.3.0/registtro/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-01-07 02:25:11.000000 registtro-1.3.0/registtro/_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     7721 2023-01-07 02:25:11.000000 registtro-1.3.0/registtro/_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-07 02:25:11.000000 registtro-1.3.0/registtro/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 02:25:29.592619 registtro-1.3.0/registtro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-01-07 02:25:29.000000 registtro-1.3.0/registtro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-01-07 02:25:29.000000 registtro-1.3.0/registtro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 02:25:29.000000 registtro-1.3.0/registtro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-07 02:25:29.000000 registtro-1.3.0/registtro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-07 02:25:29.000000 registtro-1.3.0/registtro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-07 02:25:11.000000 registtro-1.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-01-07 02:25:11.000000 registtro-1.3.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-01-07 02:25:29.596619 registtro-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-01-07 02:25:11.000000 registtro-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 02:25:29.592619 registtro-1.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-01-07 02:25:11.000000 registtro-1.3.0/tests/test_registtro.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-01-07 02:25:11.000000 registtro-1.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:28:24.552386 registtro-1.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:28:24.540386 registtro-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:28:24.548386 registtro-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-19 16:28:08.000000 registtro-1.4.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-19 16:28:08.000000 registtro-1.4.0/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-19 16:28:08.000000 registtro-1.4.0/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-19 16:28:08.000000 registtro-1.4.0/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-04-19 16:28:08.000000 registtro-1.4.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-19 16:28:08.000000 registtro-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-19 16:28:08.000000 registtro-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-19 16:28:24.552386 registtro-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4775 2023-04-19 16:28:08.000000 registtro-1.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:28:24.544386 registtro-1.4.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:28:24.548386 registtro-1.4.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:28:24.548386 registtro-1.4.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-04-19 16:28:08.000000 registtro-1.4.0/docs/source/_static/registtro.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-04-19 16:28:08.000000 registtro-1.4.0/docs/source/_static/registtro_white.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:28:24.548386 registtro-1.4.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-19 16:28:08.000000 registtro-1.4.0/docs/source/api/registtro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-19 16:28:08.000000 registtro-1.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-19 16:28:08.000000 registtro-1.4.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:28:24.548386 registtro-1.4.0/registtro/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-19 16:28:08.000000 registtro-1.4.0/registtro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-19 16:28:08.000000 registtro-1.4.0/registtro/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-19 16:28:08.000000 registtro-1.4.0/registtro/_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8466 2023-04-19 16:28:08.000000 registtro-1.4.0/registtro/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 16:28:08.000000 registtro-1.4.0/registtro/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:28:24.552386 registtro-1.4.0/registtro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-19 16:28:24.000000 registtro-1.4.0/registtro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-19 16:28:24.000000 registtro-1.4.0/registtro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:28:24.000000 registtro-1.4.0/registtro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 16:28:24.000000 registtro-1.4.0/registtro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 16:28:24.000000 registtro-1.4.0/registtro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-19 16:28:08.000000 registtro-1.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-19 16:28:08.000000 registtro-1.4.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-19 16:28:24.552386 registtro-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-19 16:28:08.000000 registtro-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:28:24.552386 registtro-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-19 16:28:08.000000 registtro-1.4.0/tests/test_registtro.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-19 16:28:08.000000 registtro-1.4.0/tox.ini
```

### Comparing `registtro-1.3.0/.github/workflows/docs.yml` & `registtro-1.4.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `registtro-1.3.0/.github/workflows/lint.yml` & `registtro-1.4.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `registtro-1.3.0/.github/workflows/mypy.yml` & `registtro-1.4.0/.github/workflows/mypy.yml`

 * *Files identical despite different names*

### Comparing `registtro-1.3.0/.github/workflows/pypi.yml` & `registtro-1.4.0/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `registtro-1.3.0/.github/workflows/tests.yml` & `registtro-1.4.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `registtro-1.3.0/LICENSE` & `registtro-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `registtro-1.3.0/PKG-INFO` & `registtro-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: registtro
-Version: 1.3.0
+Version: 1.4.0
 Summary: Weak entry, strong value immutable registry data structure.
 Home-page: https://github.com/brunonicko/registtro
 Author: Bruno Nicko
 Author-email: brunonicko@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,24 +41,28 @@
    :target: https://pepy.tech/project/registtro
 
 .. image:: https://img.shields.io/pypi/pyversions/registtro?color=light-green&style=flat
    :target: https://pypi.org/project/registtro/
 
 Overview
 --------
-Weak entry, strong value immutable registry data structure. Think of it as an immutable `WeakKeyDictionary`.
+Weak entry, strong value immutable registry data structure.
+Think of it as an immutable `WeakKeyDictionary` that efficiently evolves into a new
+copy everytime you want to make a change to it.
 
 Motivation
 ----------
-Immutable data structures are great for when you need to implement some kind of "snapshot" of states for easy undo/redo,
-time-travelling functionality. The library `pyrsistent <https://pypi.org/project/pyrsistent/>`_ is great for that, but
+Immutable data structures are great for when you need to implement some kind of
+"snapshot" of states for easy undo/redo, time-travelling functionality.
+The library `pyrsistent <https://pypi.org/project/pyrsistent/>`_ is great for that, but
 it lacks a map-like structure in which the keys are stored as weak references.
 
-`Registtro` is an implementation of that structure, which allows for proper garbage collection of the keys/entries,
-while still allowing to store their states in a centralized, immutable structure.
+`Registtro` is an implementation of that structure, which allows for proper garbage
+collection of the keys/entries, while still allowing to store their states in a
+centralized, immutable structure.
 
 Example
 -------
 Simple implementation of an undoable store that keeps track of states for entries.
 
 .. code:: python
```

### Comparing `registtro-1.3.0/README.rst` & `registtro-1.4.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 .. logo_start
 .. raw:: html
 
    <p align="center">
      <a href="https://github.com/brunonicko/registtro">
          <picture>
             <object data="./_static/registtro.svg" type="image/png">
-                <source srcset="./docs/source/_static/registtro_white.svg" media="(prefers-color-scheme: dark)">
-                <img src="./docs/source/_static/registtro.svg" width="60%" alt="registtro" />
+                <source
+                    srcset="./docs/source/_static/registtro_white.svg"
+                    media="(prefers-color-scheme: dark)"
+                />
+                <img
+                    src="./docs/source/_static/registtro.svg"
+                    width="60%"
+                    alt="registtro"
+                />
             </object>
          </picture>
      </a>
    </p>
 .. logo_end
 
 .. image:: https://github.com/brunonicko/registtro/workflows/MyPy/badge.svg
@@ -32,24 +39,28 @@
    :target: https://pepy.tech/project/registtro
 
 .. image:: https://img.shields.io/pypi/pyversions/registtro?color=light-green&style=flat
    :target: https://pypi.org/project/registtro/
 
 Overview
 --------
-Weak entry, strong value immutable registry data structure. Think of it as an immutable `WeakKeyDictionary`.
+Weak entry, strong value immutable registry data structure.
+Think of it as an immutable `WeakKeyDictionary` that efficiently evolves into a new
+copy everytime you want to make a change to it.
 
 Motivation
 ----------
-Immutable data structures are great for when you need to implement some kind of "snapshot" of states for easy undo/redo,
-time-travelling functionality. The library `pyrsistent <https://pypi.org/project/pyrsistent/>`_ is great for that, but
+Immutable data structures are great for when you need to implement some kind of
+"snapshot" of states for easy undo/redo, time-travelling functionality.
+The library `pyrsistent <https://pypi.org/project/pyrsistent/>`_ is great for that, but
 it lacks a map-like structure in which the keys are stored as weak references.
 
-`Registtro` is an implementation of that structure, which allows for proper garbage collection of the keys/entries,
-while still allowing to store their states in a centralized, immutable structure.
+`Registtro` is an implementation of that structure, which allows for proper garbage
+collection of the keys/entries, while still allowing to store their states in a
+centralized, immutable structure.
 
 Example
 -------
 Simple implementation of an undoable store that keeps track of states for entries.
 
 .. code:: python
```

### Comparing `registtro-1.3.0/docs/source/_static/registtro.svg` & `registtro-1.4.0/docs/source/_static/registtro.svg`

 * *Files identical despite different names*

### Comparing `registtro-1.3.0/docs/source/_static/registtro_white.svg` & `registtro-1.4.0/docs/source/_static/registtro_white.svg`

 * *Files identical despite different names*

### Comparing `registtro-1.3.0/docs/source/conf.py` & `registtro-1.4.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `registtro-1.3.0/registtro/_protocol.py` & `registtro-1.4.0/registtro/_protocol.py`

 * *Files identical despite different names*

### Comparing `registtro-1.3.0/registtro/_registry.py` & `registtro-1.4.0/registtro/_registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import copy
 import functools
+from weakref import WeakSet, ref
 
 import pyrsistent
 import six
 from basicco import SlottedBase, runtime_final
 from pyrsistent.typing import PMap, PMapEvolver
 from tippo import (
     AbstractSet,
+    Any,
+    Callable,
     Dict,
     Generic,
     Mapping,
+    Tuple,
+    Type,
     TypeVar,
     Union,
-    WeakSet,
     cast,
-    ref,
 )
 
 from ._exceptions import EntryNotFoundError
 
 _ET = TypeVar("_ET")
 _VT = TypeVar("_VT")
 _ST = TypeVar("_ST")
@@ -30,35 +33,38 @@
 
     __slots__ = ("__previous", "__registries", "__data")
 
     def __init__(self, initial=None):
         # type: (Union[Mapping[_ET, _VT], None]) -> None
         self.__previous = None  # type: Union[ref[Registry[_ET, _VT]], None]
         self.__registries = WeakSet({self})  # type: WeakSet[Registry[_ET, _VT]]
-        self.__data = cast(PMapEvolver[ref[_ET], _VT], pyrsistent.pmap().evolver())
+        self.__data = cast("PMapEvolver[ref[_ET], _VT]", pyrsistent.pmap().evolver())
         if initial is not None:
             self.__initialize(initial)
 
     def __contains__(self, entry):
         # type: (object) -> bool
         return ref(entry) in self.__data.persistent()
 
     def __reduce__(self):
+        # type: () -> Tuple[Type[Registry[_ET, _VT]], Tuple[Dict[_ET, _VT]]]
         return type(self), (self.to_dict(),)
 
     def __deepcopy__(self, memo=None):
+        # type: (Union[Dict[int, Any], None]) -> Registry[_ET, _VT]
         if memo is None:
             memo = {}
         try:
             deep_copy = memo[id(self)]
         except KeyError:
             deep_copy = memo[id(self)] = Registry(copy.deepcopy(self.to_dict(), memo))
-        return deep_copy
+        return cast(Registry[_ET, _VT], deep_copy)
 
     def __copy__(self):
+        # type: () -> Registry[_ET, _VT]
         return self
 
     @staticmethod
     def __clean(registries, weak_key):
         # type: (AbstractSet[Registry[_ET, _VT]], ref[_ET]) -> None
         for registry in registries:
             del registry.__data[weak_key]
@@ -142,41 +148,44 @@
 @runtime_final.final
 class RegistryEvolver(SlottedBase, Generic[_ET, _VT]):
     """Mutable registry evolver."""
 
     __slots__ = ("__registry", "__updates")
 
     def __init__(self, registry=None):
-        # type: (Union[Registry, None]) -> None
+        # type: (Union[Registry[_ET, _VT], None]) -> None
         if registry is None:
             registry = Registry()
         self.__registry = registry  # type: Registry[_ET, _VT]
         self.__updates = pyrsistent.pmap()  # type: PMap[_ET, _VT]
 
     def __contains__(self, entry):
         # type: (object) -> bool
         return entry in self.__updates or entry in self.__registry
 
     def __reduce__(self):
+        # type: () -> Tuple[_EvolverReducer[_ET, _VT], _EvolverReducerArgs[_ET, _VT]]
         return _evolver_reducer, (self.__registry, self.__updates)
 
     def __deepcopy__(self, memo=None):
+        # type: (Union[Dict[int, Any], None]) -> RegistryEvolver[_ET, _VT]
         if memo is None:
             memo = {}
         try:
             deep_copy = memo[id(self)]
         except KeyError:
             deep_copy = memo[id(self)] = RegistryEvolver.__new__(RegistryEvolver)
             deep_copy_args_a = self.__registry, memo
             deep_copy.__registry = copy.deepcopy(*deep_copy_args_a)
             deep_copy_args_b = self.__updates, memo
             deep_copy.__updates = copy.deepcopy(*deep_copy_args_b)
-        return deep_copy
+        return cast(RegistryEvolver[_ET, _VT], deep_copy)
 
     def __copy__(self):
+        # type: () -> RegistryEvolver[_ET, _VT]
         return self.fork()
 
     def update(self, updates):
         # type: (Mapping[_ET, _VT]) -> RegistryEvolver[_ET, _VT]
         """Update entries."""
         self.__updates = self.__updates.update(updates)
         return self
@@ -226,18 +235,20 @@
 
     def is_dirty(self):
         # type: () -> bool
         """Whether has updates that were not committed."""
         return bool(self.__updates)
 
     def reset(self):
+        # type: () -> None
         """Reset updates to last commit."""
         self.__updates = pyrsistent.pmap()
 
     def commit(self):
+        # type: () -> None
         """Commit updates."""
         self.__registry = self.__registry.update(self.__updates)
         self.__updates = pyrsistent.pmap()
 
     @property
     def updates(self):
         # type: () -> PMap[_ET, _VT]
@@ -246,7 +257,13 @@
 
 
 def _evolver_reducer(registry, updates):
     # type: (Registry[_ET, _VT], Mapping[_ET, _VT]) -> RegistryEvolver[_ET, _VT]
     evolver = RegistryEvolver(registry)  # type: RegistryEvolver[_ET, _VT]
     evolver.update(updates)
     return evolver
+
+
+_EvolverReducer = Callable[
+    [Registry[_ET, _VT], Mapping[_ET, _VT]], RegistryEvolver[_ET, _VT]
+]
+_EvolverReducerArgs = Tuple[Registry[_ET, _VT], Mapping[_ET, _VT]]
```

### Comparing `registtro-1.3.0/registtro.egg-info/PKG-INFO` & `registtro-1.4.0/registtro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: registtro
-Version: 1.3.0
+Version: 1.4.0
 Summary: Weak entry, strong value immutable registry data structure.
 Home-page: https://github.com/brunonicko/registtro
 Author: Bruno Nicko
 Author-email: brunonicko@gmail.com
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -41,24 +41,28 @@
    :target: https://pepy.tech/project/registtro
 
 .. image:: https://img.shields.io/pypi/pyversions/registtro?color=light-green&style=flat
    :target: https://pypi.org/project/registtro/
 
 Overview
 --------
-Weak entry, strong value immutable registry data structure. Think of it as an immutable `WeakKeyDictionary`.
+Weak entry, strong value immutable registry data structure.
+Think of it as an immutable `WeakKeyDictionary` that efficiently evolves into a new
+copy everytime you want to make a change to it.
 
 Motivation
 ----------
-Immutable data structures are great for when you need to implement some kind of "snapshot" of states for easy undo/redo,
-time-travelling functionality. The library `pyrsistent <https://pypi.org/project/pyrsistent/>`_ is great for that, but
+Immutable data structures are great for when you need to implement some kind of
+"snapshot" of states for easy undo/redo, time-travelling functionality.
+The library `pyrsistent <https://pypi.org/project/pyrsistent/>`_ is great for that, but
 it lacks a map-like structure in which the keys are stored as weak references.
 
-`Registtro` is an implementation of that structure, which allows for proper garbage collection of the keys/entries,
-while still allowing to store their states in a centralized, immutable structure.
+`Registtro` is an implementation of that structure, which allows for proper garbage
+collection of the keys/entries, while still allowing to store their states in a
+centralized, immutable structure.
 
 Example
 -------
 Simple implementation of an undoable store that keeps track of states for entries.
 
 .. code:: python
```

### Comparing `registtro-1.3.0/registtro.egg-info/SOURCES.txt` & `registtro-1.4.0/registtro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `registtro-1.3.0/setup.py` & `registtro-1.4.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 import os
 
-import setuptools  # type: ignore
+import setuptools
 
 with open("README.rst", "r") as fh:
     long_description_lines = fh.read().split("\n")
 
     line_nos = {}
     for i, line in enumerate(long_description_lines):
         if line == ".. logo_start":
             line_nos["logo_start"] = i
         elif line == ".. logo_end":
             line_nos["logo_end"] = i
             break
 
     assert line_nos["logo_start"] < line_nos["logo_end"]
 
-    long_description = "Registtro\n=========\n" + "\n".join(long_description_lines[line_nos["logo_end"] + 1 :])
+    long_description = "Registtro\n=========\n" + "\n".join(
+        long_description_lines[line_nos["logo_end"] + 1 :]
+    )
 
 
 with open("requirements.txt", "r") as fh:
     install_requires = [line.strip(os.linesep) for line in fh.readlines()]
 
 
 setuptools.setup(
     name="registtro",
-    version="1.3.0",
+    version="1.4.0",
     author="Bruno Nicko",
     author_email="brunonicko@gmail.com",
     description="Weak entry, strong value immutable registry data structure.",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/brunonicko/registtro",
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
@@ -42,10 +44,12 @@
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
-    python_requires=">= 2.7, != 3.0.*, != 3.1.*, != 3.2.*, != 3.3.*, != 3.4.*, != 3.5.*, != 3.6.*",
+    python_requires=(
+        ">= 2.7, != 3.0.*, != 3.1.*, != 3.2.*, != 3.3.*, != 3.4.*, != 3.5.*, != 3.6.*"
+    ),
     tests_require=["pytest"],
 )
```

### Comparing `registtro-1.3.0/tests/test_registtro.py` & `registtro-1.4.0/tests/test_registtro.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,17 @@
     assert registry.to_dict() == evolver.to_dict()
 
     new_registry = new_evolver.get_registry()
     assert new_registry.to_dict() == new_evolver.to_dict()
     assert new_registry.to_dict() == {entry_a: 1, entry_b: 2, entry_c: 3}
 
 
-@pytest.mark.parametrize("deep_copier", (copy.deepcopy, lambda s: pickle.loads(pickle.dumps(s))))
+@pytest.mark.parametrize(
+    "deep_copier", (copy.deepcopy, lambda s: pickle.loads(pickle.dumps(s)))
+)
 def test_deep_copy_and_pickle_registry(deep_copier):
     class _Entry:
         __name__ = __qualname__ = "_Entry"
 
         def __init__(self, name):
             self.name = name
 
@@ -148,15 +150,17 @@
 
     copied_entries, copied_registry = deep_copier((entries, registry))
     truth_dict = registry.to_dict()
     del truth_dict[entry_d]
     assert copied_registry.to_dict() == truth_dict
 
 
-@pytest.mark.parametrize("deep_copier", (copy.deepcopy, lambda s: pickle.loads(pickle.dumps(s))))
+@pytest.mark.parametrize(
+    "deep_copier", (copy.deepcopy, lambda s: pickle.loads(pickle.dumps(s)))
+)
 def test_deep_copy_and_pickle_evolver(deep_copier):
     class _Entry:
         __name__ = __qualname__ = "_Entry"
 
         def __init__(self, name):
             self.name = name
 
@@ -169,15 +173,19 @@
     globals()[_Entry.__name__] = _Entry
 
     entry_a = _Entry("a")
     entry_b = _Entry("b")
     entry_c = _Entry("c")
     entry_d = _Entry("d")
     entries = (entry_a,)
-    evolver = Registry({entry_a: 1, entry_d: 4}).get_evolver().update({entry_b: 2, entry_c: 3})
+    evolver = (
+        Registry({entry_a: 1, entry_d: 4})
+        .get_evolver()
+        .update({entry_b: 2, entry_c: 3})
+    )
 
     copied_entries, copied_evolver = deep_copier((entries, evolver))
     assert len(copied_evolver.to_dict()) == 3
     truth_dict = evolver.to_dict()
     del truth_dict[entry_d]
     assert copied_evolver.to_dict() == truth_dict
```


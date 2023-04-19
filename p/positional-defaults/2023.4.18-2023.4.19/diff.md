# Comparing `tmp/positional_defaults-2023.4.18.tar.gz` & `tmp/positional_defaults-2023.4.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "positional_defaults-2023.4.18.tar", last modified: Tue Apr 18 10:14:31 2023, max compression
+gzip compressed data, was "positional_defaults-2023.4.19.tar", last modified: Wed Apr 19 12:28:17 2023, max compression
```

## Comparing `positional_defaults-2023.4.18.tar` & `positional_defaults-2023.4.19.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 ntessore   (501) staff       (20)        0 2023-04-18 10:14:31.153699 positional_defaults-2023.4.18/
--rw-r--r--   0 ntessore   (501) staff       (20)     1072 2023-04-15 03:02:05.000000 positional_defaults-2023.4.18/LICENSE.txt
--rw-r--r--   0 ntessore   (501) staff       (20)     2418 2023-04-18 10:14:31.153296 positional_defaults-2023.4.18/PKG-INFO
--rw-r--r--   0 ntessore   (501) staff       (20)     1844 2023-04-17 09:34:00.000000 positional_defaults-2023.4.18/README.md
--rw-r--r--   0 ntessore   (501) staff       (20)      820 2023-04-18 09:58:09.000000 positional_defaults-2023.4.18/_positional_defaults.py
-drwxr-xr-x   0 ntessore   (501) staff       (20)        0 2023-04-18 10:14:31.152612 positional_defaults-2023.4.18/positional_defaults.egg-info/
--rw-r--r--   0 ntessore   (501) staff       (20)     2418 2023-04-18 10:14:31.000000 positional_defaults-2023.4.18/positional_defaults.egg-info/PKG-INFO
--rw-r--r--   0 ntessore   (501) staff       (20)      264 2023-04-18 10:14:31.000000 positional_defaults-2023.4.18/positional_defaults.egg-info/SOURCES.txt
--rw-r--r--   0 ntessore   (501) staff       (20)        1 2023-04-18 10:14:31.000000 positional_defaults-2023.4.18/positional_defaults.egg-info/dependency_links.txt
--rw-r--r--   0 ntessore   (501) staff       (20)       41 2023-04-18 10:14:31.000000 positional_defaults-2023.4.18/positional_defaults.egg-info/top_level.txt
--rw-r--r--   0 ntessore   (501) staff       (20)     2823 2023-04-18 10:08:28.000000 positional_defaults-2023.4.18/positional_defaults.py
--rw-r--r--   0 ntessore   (501) staff       (20)      823 2023-04-18 10:14:02.000000 positional_defaults-2023.4.18/pyproject.toml
--rw-r--r--   0 ntessore   (501) staff       (20)       38 2023-04-18 10:14:31.153801 positional_defaults-2023.4.18/setup.cfg
--rw-r--r--   0 ntessore   (501) staff       (20)      692 2023-04-18 09:33:36.000000 positional_defaults-2023.4.18/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:28:17.001296 positional_defaults-2023.4.19/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-19 12:28:07.000000 positional_defaults-2023.4.19/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-19 12:28:17.001296 positional_defaults-2023.4.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-04-19 12:28:07.000000 positional_defaults-2023.4.19/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-19 12:28:07.000000 positional_defaults-2023.4.19/_positional_defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:28:17.001296 positional_defaults-2023.4.19/positional_defaults.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-19 12:28:16.000000 positional_defaults-2023.4.19/positional_defaults.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-19 12:28:16.000000 positional_defaults-2023.4.19/positional_defaults.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:28:16.000000 positional_defaults-2023.4.19/positional_defaults.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-19 12:28:16.000000 positional_defaults-2023.4.19/positional_defaults.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-19 12:28:07.000000 positional_defaults-2023.4.19/positional_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-19 12:28:07.000000 positional_defaults-2023.4.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 12:28:17.001296 positional_defaults-2023.4.19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-19 12:28:07.000000 positional_defaults-2023.4.19/setup.py
```

### Comparing `positional_defaults-2023.4.18/LICENSE.txt` & `positional_defaults-2023.4.19/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `positional_defaults-2023.4.18/PKG-INFO` & `positional_defaults-2023.4.19/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: positional_defaults
-Version: 2023.4.18
+Version: 2023.4.19
 Summary: Set defaults for any positional-only parameter
 Author-email: Nicolas Tessore <n.tessore@ucl.ac.uk>, Nathaniel Starkman <n.starkman@mail.utoronto.ca>
 License: MIT
 Project-URL: Homepage, https://github.com/ntessore/positional_defaults
 Project-URL: Issues, https://github.com/ntessore/positional_defaults/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -82,20 +82,27 @@
 >>> signature(greet)
 <Signature (greeting='Welcome', prefix='Mrs', forename='Alice', surname, /, suffix='Esq')>
 ```
 
 These show up correctly in the usual places such as `help()`:
 
 ```py
->>> help(interval)
+>>> help(myrange)
 
 Help on function myrange:
 
 myrange(start=0, stop, /, step=1)
 
 >>> help(greet)
 
 Help on function greet:
 
 greet(greeting='Welcome', prefix='Mrs', forename='Alice', surname, /, suffix='Esq')
 
 ```
+
+Performance
+-----------
+
+When the package is compiled as a native extension (which is what pip will
+deliver in the majority of cases), functions with positional defaults have
+comparable performance with respect to their undecorated functions.
```

### Comparing `positional_defaults-2023.4.18/README.md` & `positional_defaults-2023.4.19/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -68,20 +68,27 @@
 >>> signature(greet)
 <Signature (greeting='Welcome', prefix='Mrs', forename='Alice', surname, /, suffix='Esq')>
 ```
 
 These show up correctly in the usual places such as `help()`:
 
 ```py
->>> help(interval)
+>>> help(myrange)
 
 Help on function myrange:
 
 myrange(start=0, stop, /, step=1)
 
 >>> help(greet)
 
 Help on function greet:
 
 greet(greeting='Welcome', prefix='Mrs', forename='Alice', surname, /, suffix='Esq')
 
 ```
+
+Performance
+-----------
+
+When the package is compiled as a native extension (which is what pip will
+deliver in the majority of cases), functions with positional defaults have
+comparable performance with respect to their undecorated functions.
```

### Comparing `positional_defaults-2023.4.18/positional_defaults.egg-info/PKG-INFO` & `positional_defaults-2023.4.19/positional_defaults.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: positional-defaults
-Version: 2023.4.18
+Version: 2023.4.19
 Summary: Set defaults for any positional-only parameter
 Author-email: Nicolas Tessore <n.tessore@ucl.ac.uk>, Nathaniel Starkman <n.starkman@mail.utoronto.ca>
 License: MIT
 Project-URL: Homepage, https://github.com/ntessore/positional_defaults
 Project-URL: Issues, https://github.com/ntessore/positional_defaults/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -82,20 +82,27 @@
 >>> signature(greet)
 <Signature (greeting='Welcome', prefix='Mrs', forename='Alice', surname, /, suffix='Esq')>
 ```
 
 These show up correctly in the usual places such as `help()`:
 
 ```py
->>> help(interval)
+>>> help(myrange)
 
 Help on function myrange:
 
 myrange(start=0, stop, /, step=1)
 
 >>> help(greet)
 
 Help on function greet:
 
 greet(greeting='Welcome', prefix='Mrs', forename='Alice', surname, /, suffix='Esq')
 
 ```
+
+Performance
+-----------
+
+When the package is compiled as a native extension (which is what pip will
+deliver in the majority of cases), functions with positional defaults have
+comparable performance with respect to their undecorated functions.
```

### Comparing `positional_defaults-2023.4.18/positional_defaults.py` & `positional_defaults-2023.4.19/positional_defaults.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # license: MIT
 '''Set defaults for any positional-only parameter.'''
 
-__version__ = '2023.4.18'
+__version__ = '2023.4.19'
 
 __all__ = ['defaults']
 
-from functools import partial
+from functools import partial, update_wrapper
 from inspect import Parameter, Signature as _Signature
 from types import MappingProxyType
-from typing import Any, Callable, List, Tuple, TypeVar, Union, overload
+from typing import Any, Callable, TypeVar, Union, overload
 
-from _positional_defaults import ARG, wrap
+from _positional_defaults import wrap
 
 F = TypeVar('F', bound=Callable[..., Any])
 
 
+ARG = object()
+
+
 class Signature(_Signature):
     '''Signature with defaults anywhere in positional-only parameters.'''
 
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
         self.__parameters = super().parameters
 
@@ -59,35 +62,33 @@
 
     if not callable(func):
         raise TypeError('not a callable')
 
     sig = Signature.from_callable(func)
     sig.update_defaults(**_defaults)
 
-    pars = {name: par for name, par in sig.parameters.items()
-            if par.kind == par.POSITIONAL_ONLY}
-
-    n = len(pars)
+    popars = {name: par for name, par in sig.parameters.items()
+              if par.kind == par.POSITIONAL_ONLY}
 
-    fill_order = [name for name in pars if name not in _defaults]
+    fill_order = [name for name in popars if name not in _defaults]
     fill_order += list(_defaults.keys())
 
-    part_order = [[name for name in pars if name in fill_order[:k]]
-                  for k in range(n+1)]
+    part_order = [[name for name in popars if name in fill_order[:n]]
+                  for n in range(len(popars))]
 
-    _patterns: List[Tuple[object, ...]] = []
-    for k in range(n+1):
-        pattern: List[object] = []
-        for name in pars:
-            if name in part_order[k]:
+    patterns = []
+    for names in part_order:
+        pattern = []
+        for name in popars:
+            if name in names:
                 pattern.append(ARG)
             elif name in _defaults:
                 pattern.append(_defaults[name])
             else:
                 break
-        _patterns.append(tuple(pattern))
-    patterns: Tuple[Tuple[object, ...], ...] = tuple(_patterns)
+        patterns.append(tuple(pattern))
 
-    wrapper = wrap(func, patterns)
+    wrapper = wrap(func, tuple(patterns), ARG)
+    update_wrapper(wrapper, func)
     wrapper.__signature__ = sig  # type: ignore[attr-defined]
 
     return wrapper
```

### Comparing `positional_defaults-2023.4.18/pyproject.toml` & `positional_defaults-2023.4.19/pyproject.toml`

 * *Files identical despite different names*


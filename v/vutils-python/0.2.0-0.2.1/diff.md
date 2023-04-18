# Comparing `tmp/vutils-python-0.2.0.tar.gz` & `tmp/vutils-python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vutils-python-0.2.0.tar", last modified: Sun Mar  5 22:53:04 2023, max compression
+gzip compressed data, was "vutils-python-0.2.1.tar", last modified: Tue Apr 18 23:15:14 2023, max compression
```

## Comparing `vutils-python-0.2.0.tar` & `vutils-python-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:53:04.881900 vutils-python-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-05 22:52:51.000000 vutils-python-0.2.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-05 22:52:51.000000 vutils-python-0.2.0/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-05 22:52:51.000000 vutils-python-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-03-05 22:52:51.000000 vutils-python-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-03-05 22:53:04.881900 vutils-python-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-05 22:52:51.000000 vutils-python-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-05 22:52:51.000000 vutils-python-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-03-05 22:53:04.881900 vutils-python-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      282 2023-03-05 22:52:51.000000 vutils-python-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:53:04.877900 vutils-python-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:53:04.877900 vutils-python-0.2.0/src/vutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:53:04.877900 vutils-python-0.2.0/src/vutils/python/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-05 22:52:51.000000 vutils-python-0.2.0/src/vutils/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-05 22:52:51.000000 vutils-python-0.2.0/src/vutils/python/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-03-05 22:52:51.000000 vutils-python-0.2.0/src/vutils/python/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-05 22:52:51.000000 vutils-python-0.2.0/src/vutils/python/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-05 22:52:51.000000 vutils-python-0.2.0/src/vutils/python/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:53:04.881900 vutils-python-0.2.0/src/vutils_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-03-05 22:53:04.000000 vutils-python-0.2.0/src/vutils_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-05 22:53:04.000000 vutils-python-0.2.0/src/vutils_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 22:53:04.000000 vutils-python-0.2.0/src/vutils_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-05 22:53:04.000000 vutils-python-0.2.0/src/vutils_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-05 22:53:04.000000 vutils-python-0.2.0/src/vutils_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-05 22:53:04.000000 vutils-python-0.2.0/src/vutils_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:53:04.877900 vutils-python-0.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-05 22:53:04.881900 vutils-python-0.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-05 22:52:51.000000 vutils-python-0.2.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-03-05 22:52:51.000000 vutils-python-0.2.0/tests/unit/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-03-05 22:52:51.000000 vutils-python-0.2.0/tests/unit/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-03-05 22:52:51.000000 vutils-python-0.2.0/tests/unit/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-05 22:52:51.000000 vutils-python-0.2.0/tests/unit/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-03-05 22:52:51.000000 vutils-python-0.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:15:14.675327 vutils-python-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-18 23:15:02.000000 vutils-python-0.2.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-18 23:15:02.000000 vutils-python-0.2.1/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 23:15:02.000000 vutils-python-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-18 23:15:02.000000 vutils-python-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-18 23:15:14.675327 vutils-python-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-18 23:15:02.000000 vutils-python-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-18 23:15:02.000000 vutils-python-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-04-18 23:15:14.675327 vutils-python-0.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      282 2023-04-18 23:15:02.000000 vutils-python-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:15:14.671327 vutils-python-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:15:14.671327 vutils-python-0.2.1/src/vutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:15:14.675327 vutils-python-0.2.1/src/vutils/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-18 23:15:02.000000 vutils-python-0.2.1/src/vutils/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-18 23:15:02.000000 vutils-python-0.2.1/src/vutils/python/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-18 23:15:02.000000 vutils-python-0.2.1/src/vutils/python/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 23:15:02.000000 vutils-python-0.2.1/src/vutils/python/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-18 23:15:02.000000 vutils-python-0.2.1/src/vutils/python/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:15:14.675327 vutils-python-0.2.1/src/vutils_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-04-18 23:15:14.000000 vutils-python-0.2.1/src/vutils_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-18 23:15:14.000000 vutils-python-0.2.1/src/vutils_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:15:14.000000 vutils-python-0.2.1/src/vutils_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:15:14.000000 vutils-python-0.2.1/src/vutils_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-18 23:15:14.000000 vutils-python-0.2.1/src/vutils_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 23:15:14.000000 vutils-python-0.2.1/src/vutils_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:15:14.671327 vutils-python-0.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:15:14.675327 vutils-python-0.2.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-18 23:15:02.000000 vutils-python-0.2.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-18 23:15:02.000000 vutils-python-0.2.1/tests/unit/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-18 23:15:02.000000 vutils-python-0.2.1/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-18 23:15:02.000000 vutils-python-0.2.1/tox.ini
```

### Comparing `vutils-python-0.2.0/LICENSE` & `vutils-python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vutils-python-0.2.0/PKG-INFO` & `vutils-python-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python language tools
 Home-page: https://github.com/i386x/vutils-python
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-python/issues
 Project-URL: Source, https://github.com/i386x/vutils-python
```

### Comparing `vutils-python-0.2.0/README.md` & `vutils-python-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vutils-python-0.2.0/pyproject.toml` & `vutils-python-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vutils-python-0.2.0/setup.cfg` & `vutils-python-0.2.1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,18 @@
 metadata = True
 restructuredtext = False
 strict = True
 
 [sdist]
 formats = zip, gztar
 
+[coverage:report]
+exclude_lines = 
+	^if TYPE_CHECKING:$
+
 [flake8]
 filename = *.py,*.pyi,*.pyw
 select = E,F,W,C,G,Y
 enable-extensions = G,Y
 max-line-length = 79
 max-doc-length = 79
 extend-ignore = E203, E302, W503
```

### Comparing `vutils-python-0.2.0/src/vutils/python/objects.py` & `vutils-python-0.2.1/src/vutils/python/objects.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 #
 """Python objects utilities."""
 
 from typing import TYPE_CHECKING, cast
 
 if TYPE_CHECKING:
     from collections.abc import Callable, Generator, MutableMapping
+    from typing import TypeVar
 
-    from vutils.python import _KT, _VT
+    _KT = TypeVar("_KT")
+    _VT = TypeVar("_VT")
 
 
 def merge_data(dest: object, src: object) -> None:
     """
     Merge data from the source object to the destination object.
 
     :param dest: The destination object
@@ -39,52 +41,53 @@
         )
 
 
 def ensure_key(
     mapping: "MutableMapping[_KT, _VT]", key: "_KT", default: "_VT"
 ) -> None:
     """
-    Ensure <mapping> has a <key> of the same type as <default>.
+    Ensure :arg:`mapping` has a :arg:`key` of the same type as :arg:`default`.
 
     :param mapping: The mapping
     :param key: The key
-    :param default: The default value if <key> is not set
-    :raises TypeError: when the value under the <key> cannot be converted to
-        the type that has <default>
-
-    If <key> is present in <mapping>, ensure the value is of a same type as
-    <default>. Otherwise, store <default> to <mapping> under <key>.
+    :param default: The default value if :arg:`key` is not set
+    :raises TypeError: when the value under the :arg:`key` cannot be converted
+        to the type that has :arg:`default`
+
+    If :arg:`key` is present in :arg:`mapping`, ensure the value is of a same
+    type as :arg:`default`. Otherwise, store :arg:`default` to :arg:`mapping`
+    under :arg:`key`.
     """
     typecls: "type[_VT]" = type(default)
     if key in mapping and not isinstance(mapping[key], typecls):
         # Raises TypeError if conversion fails
         mapping[key] = cast("Callable[[_VT], _VT]", typecls)(mapping[key])
     if key not in mapping:
         mapping[key] = default
 
 
 def ensure_no_key(mapping: "MutableMapping[_KT, _VT]", key: "_KT") -> None:
     """
-    Ensure <key> is not present in <mapping>.
+    Ensure :arg:`key` is not present in :arg:`mapping`.
 
     :param mapping: The mapping
     :param key: The key
     """
     if key in mapping:
         del mapping[key]
 
 
 def flatten(obj: object) -> "Generator[object, None, None]":
     """
-    Flatten <obj> recursively.
+    Flatten :arg:`obj` recursively.
 
     :param obj: The object to be flattened
-    :return: the generator that yields items from flattened <obj>
+    :return: the generator that yields items from flattened :arg:`obj`
 
-    If <obj> is :class:`list` or :class:`tuple`, yield items from <obj>'s
-    flattened element. Otherwise, yield <obj>.
+    If :arg:`obj` is :class:`list` or :class:`tuple`, yield items from
+    :arg:`obj`'s flattened element. Otherwise, yield :arg:`obj`.
     """
     if isinstance(obj, (tuple, list)):
         for elem in obj:
             yield from flatten(elem)
     else:
         yield obj
```

### Comparing `vutils-python-0.2.0/src/vutils_python.egg-info/PKG-INFO` & `vutils-python-0.2.1/src/vutils_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-python
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python language tools
 Home-page: https://github.com/i386x/vutils-python
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-python/issues
 Project-URL: Source, https://github.com/i386x/vutils-python
```

### Comparing `vutils-python-0.2.0/src/vutils_python.egg-info/SOURCES.txt` & `vutils-python-0.2.1/src/vutils_python.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -15,11 +15,9 @@
 src/vutils_python.egg-info/PKG-INFO
 src/vutils_python.egg-info/SOURCES.txt
 src/vutils_python.egg-info/dependency_links.txt
 src/vutils_python.egg-info/not-zip-safe
 src/vutils_python.egg-info/requires.txt
 src/vutils_python.egg-info/top_level.txt
 tests/unit/__init__.py
-tests/unit/common.py
-tests/unit/test_coverage.py
 tests/unit/test_objects.py
 tests/unit/test_version.py
```

### Comparing `vutils-python-0.2.0/tests/unit/test_objects.py` & `vutils-python-0.2.1/tests/unit/test_objects.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,29 +2,36 @@
 # File:    ./tests/unit/test_objects.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2022-06-28 12:39:49 +0200
 # Project: vutils-python: Python language tools
 #
 # SPDX-License-Identifier: MIT
 #
-"""Test `vutils.python.objects` module."""
+"""
+Test :mod:`vutils.python.objects` module.
+
+.. |merge_data| replace:: :func:`~vutils.python.objects.merge_data`
+.. |ensure_key| replace:: :func:`~vutils.python.objects.ensure_key`
+.. |ensure_no_key| replace:: :func:`~vutils.python.objects.ensure_no_key`
+.. |flatten| replace:: :func:`~vutils.python.objects.flatten`
+"""
 
 from vutils.testing.testcase import TestCase
 from vutils.testing.utils import make_type
 
 from vutils.python.objects import (
     ensure_key,
     ensure_no_key,
     flatten,
     merge_data,
 )
 
 
 class MergeDataTestCase(TestCase):
-    """Test case for `merge_data`."""
+    """Test case for |merge_data|."""
 
     __slots__ = ()
 
     def test_merge_lists(self):
         """Test merging two lists."""
         src = [1, 2, "a"]
         dest = [1, "b"]
@@ -68,15 +75,15 @@
             merge_data([], {1, 2})
 
         with self.assertRaises(TypeError):
             merge_data(b_type(), a_type())
 
 
 class EnsureKeyTestCase(TestCase):
-    """Test case for `ensure_key`."""
+    """Test case for |ensure_key|."""
 
     __slots__ = ()
 
     def test_key_desired_type(self):
         """Test that a key exists and the value has desired type."""
         mapping = {"a": 1}
 
@@ -106,29 +113,29 @@
         mapping = {"a": 1}
 
         ensure_key(mapping, "b", 2)
         self.assertEqual(mapping["b"], 2)
 
 
 class EnsureNoKeyTestCase(TestCase):
-    """Test case for `ensure_no_key`."""
+    """Test case for |ensure_no_key|."""
 
     __slots__ = ()
 
     def test_ensure_no_key(self):
         """Test the key is removed."""
         mapping = {"a": 1}
 
         for key in ("a", "b"):
             ensure_no_key(mapping, key)
             self.assertNotIn(key, mapping)
 
 
 class FlattenTestCase(TestCase):
-    """Test case for `flatten`."""
+    """Test case for |flatten|."""
 
     __slots__ = ()
 
     def test_flatten_simple_objects(self):
         """Test simple objects flattening."""
         self.assertEqual(list(flatten(1)), [1])
         self.assertEqual(list(flatten("abc")), ["abc"])
```

### Comparing `vutils-python-0.2.0/tests/unit/test_version.py` & `vutils-python-0.2.1/tests/unit/test_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # File:    ./tests/unit/test_version.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2022-06-24 14:03:43 +0200
 # Project: vutils-python: Python language tools
 #
 # SPDX-License-Identifier: MIT
 #
-"""Test `vutils.python.version` module."""
+"""Test :mod:`vutils.python.version` module."""
 
 from vutils.testing.testcase import TestCase
 
 from vutils.python.version import __version__
 
 
 class VersionTestCase(TestCase):
```

### Comparing `vutils-python-0.2.0/tox.ini` & `vutils-python-0.2.1/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 # Project: vutils-python: Python language tools
 # Brief:   Configuration for tox
 #
 # SPDX-License-Identifier: MIT
 #
 
 [tox]
+requires =
+    pip >= 19.2
+    setuptools >= 65.5.1
+    wheel >= 0.38.1
 envlist =
     py{37,38,39,310}, linters
 skip_missing_interpreters = True
 
 [testenv]
 passenv = *
 description =
     {envname}: Run unit tests for {envname}
 deps =
-    pip >= 19.2
-    setuptools >= 65.5.1
-    wheel >= 0.38.1
     safety
     pytest
     pytest-cov
-    pytest-order
     vutils-testing
     coveralls
 commands =
     safety check --full-report
     pytest -v --cov=vutils.python --cov-report=term-missing tests
     {env:COVERALLS_CMD:coveralls --output={envname}-coverage.txt}
```


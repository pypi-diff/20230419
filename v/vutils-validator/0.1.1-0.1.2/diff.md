# Comparing `tmp/vutils-validator-0.1.1.tar.gz` & `tmp/vutils-validator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vutils-validator-0.1.1.tar", last modified: Mon Mar  6 11:13:23 2023, max compression
+gzip compressed data, was "vutils-validator-0.1.2.tar", last modified: Wed Apr 19 13:48:26 2023, max compression
```

## Comparing `vutils-validator-0.1.1.tar` & `vutils-validator-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:13:23.326379 vutils-validator-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/ChangeLog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-03-06 11:13:23.326379 vutils-validator-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-03-06 11:13:23.326379 vutils-validator-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:13:23.318379 vutils-validator-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:13:23.318379 vutils-validator-0.1.1/src/vutils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:13:23.322379 vutils-validator-0.1.1/src/vutils/validator/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/src/vutils/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/src/vutils/validator/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/src/vutils/validator/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/src/vutils/validator/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/src/vutils/validator/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/src/vutils/validator/value.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/src/vutils/validator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:13:23.322379 vutils-validator-0.1.1/src/vutils_validator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-03-06 11:13:23.000000 vutils-validator-0.1.1/src/vutils_validator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-06 11:13:23.000000 vutils-validator-0.1.1/src/vutils_validator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 11:13:23.000000 vutils-validator-0.1.1/src/vutils_validator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 11:13:23.000000 vutils-validator-0.1.1/src/vutils_validator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-06 11:13:23.000000 vutils-validator-0.1.1/src/vutils_validator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-06 11:13:23.000000 vutils-validator-0.1.1/src/vutils_validator.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:13:23.318379 vutils-validator-0.1.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:13:23.326379 vutils-validator-0.1.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/tests/unit/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/tests/unit/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/tests/unit/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/tests/unit/test_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/tests/unit/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-03-06 11:13:09.000000 vutils-validator-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.521265 vutils-validator-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/ChangeLog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-19 13:48:26.521265 vutils-validator-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-19 13:48:26.521265 vutils-validator-0.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      292 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.513265 vutils-validator-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.513265 vutils-validator-0.1.2/src/vutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.517265 vutils-validator-0.1.2/src/vutils/validator/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/src/vutils/validator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.521265 vutils-validator-0.1.2/src/vutils_validator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-04-19 13:48:26.000000 vutils-validator-0.1.2/src/vutils_validator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-19 13:48:26.000000 vutils-validator-0.1.2/src/vutils_validator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:48:26.000000 vutils-validator-0.1.2/src/vutils_validator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 13:48:26.000000 vutils-validator-0.1.2/src/vutils_validator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-19 13:48:26.000000 vutils-validator-0.1.2/src/vutils_validator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 13:48:26.000000 vutils-validator-0.1.2/src/vutils_validator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.513265 vutils-validator-0.1.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 13:48:26.521265 vutils-validator-0.1.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/tests/unit/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/tests/unit/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3696 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/tests/unit/test_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/tests/unit/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4061 2023-04-19 13:48:08.000000 vutils-validator-0.1.2/tox.ini
```

### Comparing `vutils-validator-0.1.1/LICENSE` & `vutils-validator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.1/PKG-INFO` & `vutils-validator-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-validator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Data validation utilities
 Home-page: https://github.com/i386x/vutils-validator
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-validator/issues
 Project-URL: Source, https://github.com/i386x/vutils-validator
```

### Comparing `vutils-validator-0.1.1/README.md` & `vutils-validator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.1/pyproject.toml` & `vutils-validator-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vutils-validator-0.1.1/setup.cfg` & `vutils-validator-0.1.2/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -58,14 +58,18 @@
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

### Comparing `vutils-validator-0.1.1/src/vutils/validator/basic.py` & `vutils-validator-0.1.2/src/vutils/validator/basic.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,54 +2,58 @@
 # File:    ./src/vutils/validator/basic.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2022-05-29 21:59:20 +0200
 # Project: vutils-validator: Data validation utilities
 #
 # SPDX-License-Identifier: MIT
 #
-"""Basic validation."""
+"""
+Basic validation.
+
+:const EMAIL_RE: The simple regular expression matching email address
+"""
 
 import re
 from typing import TYPE_CHECKING
 
 from vutils.validator.errors import ValidationError
 
 if TYPE_CHECKING:
     from vutils.validator.value import ValueHolder
 
-EMAIL_RE = r"^\S+@\S+\.[A-Za-z]+$"
+EMAIL_RE: str = r"^\S+@\S+\.[A-Za-z]+$"
 
 
 def verify_not_empty(value: "ValueHolder | str") -> None:
     """
-    Verify that value is not empty.
+    Verify that :arg:`value` is not empty.
 
     :param value: The value to be verified
-    :raises ValidationError: when verification fails
+    :raises ~vutils.validator.errors.ValidationError: when verification fails
     """
     if len(str(value)) == 0:
         raise ValidationError("must not be empty!", value)
 
 
 def verify_matches(
     value: "ValueHolder | str", regex: str, detail: str = ""
 ) -> None:
     """
-    Verify that value matches the regular expression.
+    Verify that :arg:`value` matches the regular expression.
 
     :param value: The value to be verified
     :param regex: The regular expression
     :param detail: The error detail (default is ``must match `{regex}`!``)
-    :raises ValidationError: when verification fails
+    :raises ~vutils.validator.errors.ValidationError: when verification fails
     """
     if not re.match(regex, str(value)):
         raise ValidationError(detail or f"must match `{regex}`!", value)
 
 
 def verify_email(value: "ValueHolder | str") -> None:
     """
-    Verify that value is an email address.
+    Verify that :arg:`value` is an email address.
 
     :param value: The value to be verified
-    :raises ValidationError: when verification fails
+    :raises ~vutils.validator.errors.ValidationError: when verification fails
     """
     verify_matches(value, EMAIL_RE, "must be an email address!")
```

### Comparing `vutils-validator-0.1.1/src/vutils/validator/errors.py` & `vutils-validator-0.1.2/src/vutils/validator/errors.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,16 +8,23 @@
 #
 """Validation errors."""
 
 from vutils.validator.value import ValueHolder
 
 
 class ValidationError(Exception):
-    """Used to report failed checks."""
+    """
+    Used to report failed checks.
 
+    :ivar message: The reason of the error
+    :ivar value: The value that issued the error
+    """
+
+    message: str
+    value: ValueHolder
     __slots__ = ("message", "value")
 
     def __init__(self, message: str, value: "ValueHolder | str") -> None:
         """
         Initialize the error object.
 
         :param message: The error message
@@ -35,12 +42,12 @@
 
         :return: the error representation
         """
         return self.value.detail(self.message)
 
     def __str__(self) -> str:
         """
-        Get the error representation (`str` alias).
+        Get the error representation (:class:`str` alias).
 
         :return: the error representation
         """
         return repr(self)
```

### Comparing `vutils-validator-0.1.1/src/vutils/validator/value.py` & `vutils-validator-0.1.2/src/vutils/validator/value.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,45 +11,54 @@
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     import pathlib
 
 
 class Location:
-    """Hold value/token location."""
+    """
+    Hold the token's location.
 
+    :ivar path: The path to the token's origin
+    :ivar line: The line number of the token's origin
+    :ivar column: The column number of the token's origin
+    """
+
+    path: "str | pathlib.Path | None"
+    line: int
+    column: int
     __slots__ = ("path", "line", "column")
 
     def __init__(
         self,
         path: "str | pathlib.Path | None" = None,
         line: int = -1,
         column: int = -1,
     ) -> None:
         """
         Initialize the location.
 
-        :param path: The path to the file of the value/token origin
-        :param line: The line number of the value/token origin
-        :param column: The column number of the value/token origin
+        :param path: The path to the file of the token's origin
+        :param line: The line number of the token's origin
+        :param column: The column number of the token's origin
         """
         self.path = path
         self.line = line
         self.column = column
 
     def __str__(self) -> str:
         """
-        Give the string representation of the value/token location.
+        Give the string representation of the token's location.
 
-        :return: the value/token location as a `str` object
+        :return: the token's location as a :class:`str` object
 
         Location is of the form ``{path}:{line}:{column}``, where ``path``,
-        ``line``, and ``column`` are omitted together with redundant ``:`` if
-        they are `None`, negative, and negative, respectively. If ``line`` is
-        negative and ``column`` is not, the result is ``{path}:?:{column}``.
+        ``line``, and ``column`` are omitted, together with redundant ``:``, if
+        they are :obj:`None`, negative, and negative, respectively. If ``line``
+        is negative and ``column`` is not, the result is ``{path}:?:{column}``.
         """
         location: str = ""
         if self.path is not None:
             location += f"{self.path}"
         if self.line >= 0:
             if location:
                 location += ":"
@@ -60,30 +69,39 @@
             if self.line < 0:
                 location += "?:"
             location += f"{self.column}"
         return location
 
 
 class ValueHolder:
-    """Hold value with its context."""
+    """
+    Hold a value together with its context.
 
+    :ivar value: The value
+    :ivar name: The name of the value to be displayed in messages
+    :ivar location: The location of the value's origin
+    """
+
+    value: str
+    name: str
+    location: "Location | None"
     __slots__ = ("value", "name", "location")
 
     def __init__(
         self,
         value: str,
         name: str = "The value",
         location: "Location | None" = None,
     ) -> None:
         """
         Initialize the value holder.
 
         :param value: The value
         :param name: The name of the value
-        :param location: The location of the value origin
+        :param location: The location of the value's origin
         """
         self.value = value
         self.name = name
         self.location = location or Location()
 
     def __str__(self) -> str:
         """
@@ -96,16 +114,16 @@
     def detail(self, message: str) -> str:
         """
         Add detail information about the value to the message.
 
         :param message: The message
         :return: detail information about the value
 
-        Add the value location if present and the value name to *message* so
-        the final form is ``{location}: {name} {message}``.
+        Add the value's location if present and the value's name to
+        :arg:`message` so the final form is ``{location}: {name} {message}``.
         """
         location: str = str(self.location)
 
         detail: str = f"{self.name} {message}"
         if location:
             detail = f"{location}: {detail}"
         return detail
```

### Comparing `vutils-validator-0.1.1/src/vutils_validator.egg-info/PKG-INFO` & `vutils-validator-0.1.2/src/vutils_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vutils-validator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Data validation utilities
 Home-page: https://github.com/i386x/vutils-validator
 Author: Jiří Kučera
 Author-email: sanczes@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/i386x/vutils-validator/issues
 Project-URL: Source, https://github.com/i386x/vutils-validator
```

### Comparing `vutils-validator-0.1.1/src/vutils_validator.egg-info/SOURCES.txt` & `vutils-validator-0.1.2/src/vutils_validator.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -18,11 +18,10 @@
 src/vutils_validator.egg-info/SOURCES.txt
 src/vutils_validator.egg-info/dependency_links.txt
 src/vutils_validator.egg-info/not-zip-safe
 src/vutils_validator.egg-info/requires.txt
 src/vutils_validator.egg-info/top_level.txt
 tests/unit/__init__.py
 tests/unit/test_basic.py
-tests/unit/test_coverage.py
 tests/unit/test_errors.py
 tests/unit/test_value.py
 tests/unit/test_version.py
```

### Comparing `vutils-validator-0.1.1/tests/unit/test_basic.py` & `vutils-validator-0.1.2/tests/unit/test_basic.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,22 @@
 # File:    ./tests/unit/test_basic.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2022-06-01 18:00:18 +0200
 # Project: vutils-validator: Data validation utilities
 #
 # SPDX-License-Identifier: MIT
 #
-"""Test `vutils.validator.basic` module."""
+"""
+Test :mod:`vutils.validator.basic` module.
+
+.. |verify_not_empty| replace::
+   :func:`~vutils.validator.basic.verify_not_empty`
+.. |verify_matches| replace:: :func:`~vutils.validator.basic.verify_matches`
+.. |verify_email| replace:: :func:`~vutils.validator.basic.verify_email`
+"""
 
 from vutils.testing.testcase import TestCase
 
 from vutils.validator.basic import (
     verify_email,
     verify_matches,
     verify_not_empty,
@@ -21,25 +28,25 @@
 
 class BasicValidationTestCase(TestCase):
     """Test case for basic validation."""
 
     __slots__ = ()
 
     def test_verify_not_empty(self):
-        """Test `verify_not_empty`."""
+        """Test |verify_not_empty|."""
         self.do_test(verify_not_empty, ("",), "The value must not be empty!")
         self.do_test(
             verify_not_empty,
             (ValueHolder("", "foobar"),),
             "foobar must not be empty!",
         )
         self.do_test(verify_not_empty, ("foo",), None)
 
     def test_verify_matches(self):
-        """Test `verify_matches`."""
+        """Test |verify_matches|."""
         regex = r"^[_A-Za-z][_0-9A-Za-z]*$"
 
         self.do_test(
             verify_matches, ("-", regex), f"The value must match `{regex}`!"
         )
         self.do_test(
             verify_matches,
@@ -50,15 +57,15 @@
             verify_matches,
             (ValueHolder("-", "foobar"), regex, "must be an identifier!"),
             "foobar must be an identifier!",
         )
         self.do_test(verify_matches, ("_foo", regex), None)
 
     def test_verify_email(self):
-        """Test `verify_email`."""
+        """Test |verify_email|."""
         self.do_test(
             verify_email, ("foo@bar",), "The value must be an email address!"
         )
         self.do_test(
             verify_email,
             (ValueHolder("foo@bar", "foobar"),),
             "foobar must be an email address!",
@@ -69,18 +76,18 @@
         """
         Do the test of basic validation.
 
         :param func: The validation function
         :param args: The validation function arguments
         :param result: The expected result
 
-        Expected result set to `None` signals that the validation function
+        Expected result set to :obj:`None` signals that the validation function
         should not raise an exception. Otherwise the validation function should
-        raise `ValidationError` and its representation should match the
-        expected result.
+        raise :exc:`~vutils.validator.errors.ValidationError` and its
+        representation should match the expected result.
         """
         if result is None:
             func(*args)
             return
         with self.assertRaises(ValidationError) as context_manager:
             func(*args)
         self.assertEqual(f"{context_manager.exception}", result)
```

### Comparing `vutils-validator-0.1.1/tests/unit/test_errors.py` & `vutils-validator-0.1.2/tests/unit/test_errors.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,39 +2,43 @@
 # File:    ./tests/unit/test_errors.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2022-06-01 16:28:57 +0200
 # Project: vutils-validator: Data validation utilities
 #
 # SPDX-License-Identifier: MIT
 #
-"""Test `vutils.validator.errors` module."""
+"""
+Test :mod:`vutils.validator.errors` module.
+
+.. |ValidationError| replace:: :exc:`~vutils.validator.errors.ValidationError`
+"""
 
 from vutils.testing.testcase import TestCase
 
 from vutils.validator.errors import ValidationError
 from vutils.validator.value import Location, ValueHolder
 
 
 class ValidationErrorTestCase(TestCase):
-    """Test case for `ValidationError`."""
+    """Test case for |ValidationError|."""
 
     __slots__ = ()
 
     def test_validation_error(self):
-        """Test `ValidationError`."""
+        """Test |ValidationError|."""
         self.do_test("must be 123", "321", "The value must be 123")
         self.do_test(
             "must be 123",
             ValueHolder("321", "foo", Location("./bar.py", 1, 2)),
             "./bar.py:1:2: foo must be 123",
         )
 
     def do_test(self, message, value, result):
         """
-        Do the `ValidationError` test.
+        Do the |ValidationError| test.
 
         :param message: The message
         :param value: The value
         :param result: The expected result
         """
         with self.assertRaises(ValidationError) as context_manager:
             raise ValidationError(message, value)
```

### Comparing `vutils-validator-0.1.1/tests/unit/test_value.py` & `vutils-validator-0.1.2/tests/unit/test_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,53 +2,64 @@
 # File:    ./tests/unit/test_value.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2022-06-01 10:07:23 +0200
 # Project: vutils-validator: Data validation utilities
 #
 # SPDX-License-Identifier: MIT
 #
-"""Test `vutils.validator.value` module."""
+"""
+Test :mod:`vutils.validator.value` module.
+
+.. |Location| replace:: :class:`~vutils.validator.value.Location`
+.. |Location.__str__| replace::
+   :meth:`~vutils.validator.value.Location.__str__`
+.. |ValueHolder| replace:: :class:`~vutils.validator.value.ValueHolder`
+.. |ValueHolder.__str__| replace::
+   :meth:`~vutils.validator.value.ValueHolder.__str__`
+.. |ValueHolder.detail| replace::
+   :meth:`~vutils.validator.value.ValueHolder.detail`
+"""
 
 from vutils.testing.testcase import TestCase
 
 from vutils.validator.value import Location, ValueHolder
 
 
 class LocationTestCase(TestCase):
-    """Test case for `Location`."""
+    """Test case for |Location|."""
 
     __slots__ = ()
 
     def test_constructor_default(self):
         """
         Test initialization.
 
-        Test `Location` object initialization with default values.
+        Test |Location| object initialization with default values.
         """
         location = Location()
 
         self.assertIsNone(location.path)
         self.assertEqual(location.line, -1)
         self.assertEqual(location.column, -1)
 
     def test_constructor_custom(self):
         """
         Test initialization.
 
-        Test `Location` object initialization with custom values.
+        Test |Location| object initialization with custom values.
         """
         path, line, column = "./foo.py", 42, 7
         location = Location(path, line, column)
 
         self.assertEqual(location.path, path)
         self.assertEqual(location.line, line)
         self.assertEqual(location.column, column)
 
     def test_to_str_conversion(self):
-        """Test `Location.__str__`."""
+        """Test |Location.__str__|."""
         testset = [
             ((), ""),
             (("./foo.bar", -1, -1), "./foo.bar"),
             ((None, 42, -1), "42"),
             ((None, -1, 42), "?:42"),
             ((None, 42, 7), "42:7"),
             (("./foo", 42, -1), "./foo:42"),
@@ -57,54 +68,54 @@
         ]
 
         for item in testset:
             self.assertEqual(str(Location(*item[0])), item[1])
 
 
 class ValueHolderTestCase(TestCase):
-    """Test case for `ValueHolder`."""
+    """Test case for |ValueHolder|."""
 
     __slots__ = ()
 
     def test_constructor_default(self):
         """
         Test initialization.
 
-        Test `ValueHolder` object initialization with default values.
+        Test |ValueHolder| object initialization with default values.
         """
         value = "quux"
         holder = ValueHolder(value)
 
         self.assertEqual(holder.value, value)
         self.assertEqual(holder.name, "The value")
         self.assertIsInstance(holder.location, Location)
 
     def test_constructor_custom(self):
         """
         Test initialization.
 
-        Test `ValueHolder` object initialization with custom values.
+        Test |ValueHolder| object initialization with custom values.
         """
         value, name, location = "baz", "foo", Location()
         holder = ValueHolder(value, name, location)
 
         self.assertEqual(holder.value, value)
         self.assertEqual(holder.name, name)
         self.assertIs(holder.location, location)
 
     def test_value_extraction(self):
-        """Test `ValueHolder.__str__`."""
+        """Test |ValueHolder.__str__|."""
         value = "foobar"
         holder = ValueHolder(value)
 
         self.assertEqual(str(holder), value)
         self.assertEqual(str(holder), holder.value)
 
     def test_detail(self):
-        """Test `ValueHolder.detail`."""
+        """Test |ValueHolder.detail|."""
         testset = [
             (("baz",), "is bad", "The value is bad"),
             (("baz", "foo"), "is bad", "foo is bad"),
             (
                 ("baz", "foo", Location(None, 42, 7)),
                 "is bad",
                 "42:7: foo is bad",
```

### Comparing `vutils-validator-0.1.1/tests/unit/test_version.py` & `vutils-validator-0.1.2/tests/unit/test_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # File:    ./tests/unit/test_version.py
 # Author:  Jiří Kučera <sanczes AT gmail.com>
 # Date:    2022-05-03 21:26:33 +0200
 # Project: vutils-validator: Data validation utilities
 #
 # SPDX-License-Identifier: MIT
 #
-"""Test `vutils.validator.version` module."""
+"""Test :mod:`vutils.validator.version` module."""
 
 from vutils.testing.testcase import TestCase
 
 from vutils.validator.version import __version__
 
 
 class VersionTestCase(TestCase):
```

### Comparing `vutils-validator-0.1.1/tox.ini` & `vutils-validator-0.1.2/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 # Project: vutils-validator: Data validation utilities
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
     pytest -v --cov=vutils.validator --cov-report=term-missing tests
     {env:COVERALLS_CMD:coveralls --output={envname}-coverage.txt}
```


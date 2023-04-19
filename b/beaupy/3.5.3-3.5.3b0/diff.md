# Comparing `tmp/beaupy-3.5.3.tar.gz` & `tmp/beaupy-3.5.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beaupy-3.5.3.tar", max compression
+gzip compressed data, was "beaupy-3.5.3b0.tar", max compression
```

## Comparing `beaupy-3.5.3.tar` & `beaupy-3.5.3b0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1111 2023-04-19 17:19:34.820559 beaupy-3.5.3/LICENSE
--rw-r--r--   0        0        0     8118 2023-04-19 17:19:34.820559 beaupy-3.5.3/README.md
--rw-r--r--   0        0        0      260 2023-04-19 17:19:34.820559 beaupy-3.5.3/beaupy/__init__.py
--rwxr-xr-x   0        0        0    23689 2023-04-19 17:19:34.820559 beaupy-3.5.3/beaupy/_beaupy.py
--rw-r--r--   0        0        0     4059 2023-04-19 17:19:34.820559 beaupy-3.5.3/beaupy/_internals.py
--rw-r--r--   0        0        0      170 2023-04-19 17:19:34.820559 beaupy-3.5.3/beaupy/spinners/__init__.py
--rw-r--r--   0        0        0     2335 2023-04-19 17:19:34.820559 beaupy-3.5.3/beaupy/spinners/_spinners.py
--rw-r--r--   0        0        0     3662 2023-04-19 17:19:34.824560 beaupy-3.5.3/pyproject.toml
--rw-r--r--   0        0        0     9166 1970-01-01 00:00:00.000000 beaupy-3.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/LICENSE
+-rw-r--r--   0        0        0     8118 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/README.md
+-rw-r--r--   0        0        0      260 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/__init__.py
+-rwxr-xr-x   0        0        0    23689 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/_beaupy.py
+-rw-r--r--   0        0        0     4059 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/_internals.py
+-rw-r--r--   0        0        0      170 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/spinners/__init__.py
+-rw-r--r--   0        0        0     2335 2023-04-15 15:17:25.863836 beaupy-3.5.3b0/beaupy/spinners/_spinners.py
+-rw-r--r--   0        0        0     3664 2023-04-15 15:17:25.867836 beaupy-3.5.3b0/pyproject.toml
+-rw-r--r--   0        0        0     9168 1970-01-01 00:00:00.000000 beaupy-3.5.3b0/PKG-INFO
```

### Comparing `beaupy-3.5.3/LICENSE` & `beaupy-3.5.3b0/LICENSE`

 * *Files identical despite different names*

### Comparing `beaupy-3.5.3/README.md` & `beaupy-3.5.3b0/README.md`

 * *Files identical despite different names*

### Comparing `beaupy-3.5.3/beaupy/_beaupy.py` & `beaupy-3.5.3b0/beaupy/_beaupy.py`

 * *Files identical despite different names*

### Comparing `beaupy-3.5.3/beaupy/_internals.py` & `beaupy-3.5.3b0/beaupy/_internals.py`

 * *Files identical despite different names*

### Comparing `beaupy-3.5.3/beaupy/spinners/_spinners.py` & `beaupy-3.5.3b0/beaupy/spinners/_spinners.py`

 * *Files identical despite different names*

### Comparing `beaupy-3.5.3/pyproject.toml` & `beaupy-3.5.3b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'beaupy'
-version = '3.5.3'
+version = '3.5.3b0'
 description = 'A library of elements for interactive TUIs in Python'
 authors = ['Peter Vyboch <pvyboch1@gmail.com>']
 license = 'MIT'
 repository = 'https://github.com/petereon/beaupy'
 readme = 'README.md'
 keywords = ["cli", "interactive", "console", "terminal", "interface"]
 classifiers = [
```

### Comparing `beaupy-3.5.3/PKG-INFO` & `beaupy-3.5.3b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaupy
-Version: 3.5.3
+Version: 3.5.3b0
 Summary: A library of elements for interactive TUIs in Python
 Home-page: https://github.com/petereon/beaupy
 License: MIT
 Keywords: cli,interactive,console,terminal,interface
 Author: Peter Vyboch
 Author-email: pvyboch1@gmail.com
 Requires-Python: >=3.7.8,<4.0.0
```


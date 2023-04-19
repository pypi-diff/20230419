# Comparing `tmp/dahlia-2.3.1.tar.gz` & `tmp/dahlia-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dahlia-2.3.1.tar", max compression
+gzip compressed data, was "dahlia-2.3.2.tar", max compression
```

## Comparing `dahlia-2.3.1.tar` & `dahlia-2.3.2.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-01-19 17:08:30.010799 dahlia-2.3.1/LICENSE
--rw-r--r--   0        0        0     1184 2023-01-19 17:08:30.019705 dahlia-2.3.1/README.md
--rw-r--r--   0        0        0      607 2023-02-20 10:07:46.153267 dahlia-2.3.1/pyproject.toml
--rw-r--r--   0        0        0      265 2023-02-16 08:21:44.627720 dahlia-2.3.1/src/dahlia/__init__.py
--rw-r--r--   0        0        0     1097 2023-02-20 10:08:49.162665 dahlia-2.3.1/src/dahlia/__main__.py
--rw-r--r--   0        0        0     3040 2023-02-20 10:03:44.242463 dahlia-2.3.1/src/dahlia/constants.py
--rw-r--r--   0        0        0     6043 2023-01-19 17:08:30.457555 dahlia-2.3.1/src/dahlia/dahlia.py
--rw-r--r--   0        0        0     2056 2023-01-19 17:08:30.457820 dahlia-2.3.1/src/dahlia/legacy.py
--rw-r--r--   0        0        0        1 2023-01-19 17:08:30.499731 dahlia-2.3.1/src/dahlia/py.typed
--rw-r--r--   0        0        0     6574 2023-02-16 08:29:24.196625 dahlia-2.3.1/src/dahlia/utils.py
--rw-r--r--   0        0        0     1963 1970-01-01 00:00:00.000000 dahlia-2.3.1/setup.py
--rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 dahlia-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-01-19 17:08:30.010799 dahlia-2.3.2/LICENSE
+-rw-r--r--   0        0        0     1184 2023-03-14 06:05:32.029103 dahlia-2.3.2/README.md
+-rw-r--r--   0        0        0      611 2023-04-19 05:04:29.369420 dahlia-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0      265 2023-02-16 08:21:44.627720 dahlia-2.3.2/src/dahlia/__init__.py
+-rw-r--r--   0        0        0     1097 2023-04-19 05:04:35.327748 dahlia-2.3.2/src/dahlia/__main__.py
+-rw-r--r--   0        0        0     2993 2023-03-20 21:45:40.260197 dahlia-2.3.2/src/dahlia/constants.py
+-rw-r--r--   0        0        0     6044 2023-04-19 05:02:44.556635 dahlia-2.3.2/src/dahlia/dahlia.py
+-rw-r--r--   0        0        0     2056 2023-01-19 17:08:30.457820 dahlia-2.3.2/src/dahlia/legacy.py
+-rw-r--r--   0        0        0        1 2023-01-19 17:08:30.499731 dahlia-2.3.2/src/dahlia/py.typed
+-rw-r--r--   0        0        0     6574 2023-03-07 00:59:51.246219 dahlia-2.3.2/src/dahlia/utils.py
+-rw-r--r--   0        0        0     1919 1970-01-01 00:00:00.000000 dahlia-2.3.2/PKG-INFO
```

### Comparing `dahlia-2.3.1/LICENSE` & `dahlia-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dahlia-2.3.1/README.md` & `dahlia-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dahlia-2.3.1/pyproject.toml` & `dahlia-2.3.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "dahlia"
-version = "2.3.1"
+version = "2.3.2"
 description = "A library allowing you to use Minecraft format codes in strings."
 authors = ["trag1c <trag1cdev@yahoo.com>"]
 license = "MIT"
 documentation = "https://dahlia.readthedocs.io/en/latest"
-repository = "https://github.com/trag1c/Dahlia"
+repository = "https://github.com/dahlia-lib/dahlia"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.scripts]
 dahlia = "dahlia.__main__:main"
```

### Comparing `dahlia-2.3.1/src/dahlia/__main__.py` & `dahlia-2.3.2/src/dahlia/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     )
     parser.add_argument("-t", "--test", help="test the colors", action="store_true")
     parser.add_argument(
         "-v",
         "--version",
         help="print the version",
         action="version",
-        version="%(prog)s 2.3.1",
+        version="%(prog)s 2.3.2",
     )
     parser.add_argument("-c", "--clean", help="clean codes", action="store_true")
     parser.add_argument("string", nargs="?", help="the string to color", default=UNSET)
     args = parser.parse_args()
 
     d = Dahlia(depth=Depth(args.depth))
     string = args.string
```

### Comparing `dahlia-2.3.1/src/dahlia/constants.py` & `dahlia-2.3.2/src/dahlia/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,24 +122,22 @@
     (0, 255, 255): 36,  # bright cyan
     (255, 255, 255): 37,  # white
 }
 
 
 COLORS_4 = {
     **COLORS_3,
-    **{
-        (128, 128, 128): 90,  # dark gray
-        (255, 0, 0): 91,  # bright red
-        (0, 255, 0): 92,  # bright green
-        (255, 255, 0): 93,  # bright yellow
-        (0, 0, 255): 94,  # bright blue
-        (255, 0, 255): 95,  # bright magenta
-        (0, 255, 255): 96,  # bright cyan
-        (255, 255, 255): 97,  # white
-    },
+    (128, 128, 128): 90,  # dark gray
+    (255, 0, 0): 91,  # bright red
+    (0, 255, 0): 92,  # bright green
+    (255, 255, 0): 93,  # bright yellow
+    (0, 0, 255): 94,  # bright blue
+    (255, 0, 255): 95,  # bright magenta
+    (0, 255, 255): 96,  # bright cyan
+    (255, 255, 255): 97,  # white
 }
 
 FORMAT_TEMPLATES = {
     3: "\033[{}m",
     4: "\033[{}m",
     8: "\033[38;5;{}m",
     24: "\033[38;2;{};{};{}m",
```

### Comparing `dahlia-2.3.1/src/dahlia/dahlia.py` & `dahlia-2.3.2/src/dahlia/dahlia.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self.__reset = marker + "r"
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Dahlia):
             return (self.depth, self.no_reset, self.marker) == (
                 other.depth,
                 other.no_reset,
-                self.marker,
+                other.marker,
             )
         return NotImplemented
 
     def __hash__(self) -> int:
         return hash((self.depth, self.no_reset, self.marker))
 
     def __repr__(self) -> str:
```

### Comparing `dahlia-2.3.1/src/dahlia/legacy.py` & `dahlia-2.3.2/src/dahlia/legacy.py`

 * *Files identical despite different names*

### Comparing `dahlia-2.3.1/src/dahlia/utils.py` & `dahlia-2.3.2/src/dahlia/utils.py`

 * *Files identical despite different names*

### Comparing `dahlia-2.3.1/PKG-INFO` & `dahlia-2.3.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dahlia
-Version: 2.3.1
+Version: 2.3.2
 Summary: A library allowing you to use Minecraft format codes in strings.
-Home-page: https://github.com/trag1c/Dahlia
+Home-page: https://github.com/dahlia-lib/dahlia
 License: MIT
 Author: trag1c
 Author-email: trag1cdev@yahoo.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Documentation, https://dahlia.readthedocs.io/en/latest
-Project-URL: Repository, https://github.com/trag1c/Dahlia
+Project-URL: Repository, https://github.com/dahlia-lib/dahlia
 Description-Content-Type: text/markdown
 
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/dahlia)](https://pypi.python.org/pypi/dahlia)
 [![PyPI version](https://badge.fury.io/py/dahlia.svg)](https://badge.fury.io/py/dahlia)
 [![Documentation Status](https://readthedocs.org/projects/dahlia/badge/?version=latest)](https://dahlia.readthedocs.io/en/latest/?badge=latest)
 # Dahlia
```


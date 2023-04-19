# Comparing `tmp/incendium-stubs-2023.3.0.tar.gz` & `tmp/incendium-stubs-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "incendium-stubs-2023.3.0.tar", last modified: Thu Mar 30 23:56:28 2023, max compression
+gzip compressed data, was "incendium-stubs-2023.4.0.tar", last modified: Wed Apr 19 00:28:27 2023, max compression
```

## Comparing `incendium-stubs-2023.3.0.tar` & `incendium-stubs-2023.4.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:28.325766 incendium-stubs-2023.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-03-30 23:56:28.325766 incendium-stubs-2023.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-30 23:56:28.325766 incendium-stubs-2023.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:28.321766 incendium-stubs-2023.3.0/stubs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:28.325766 incendium-stubs-2023.3.0/stubs/incendium/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      619 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      832 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/dataset.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/date.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2565 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/db.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      508 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/exceptions.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:28.325766 incendium-stubs-2023.3.0/stubs/incendium/helper/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/helper/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/helper/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      320 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/helper/types.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      395 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/net.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)      259 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/tag.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/user.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/util.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:28.325766 incendium-stubs-2023.3.0/stubs/incendium/vision/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/vision/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/vision/gui.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/vision/nav.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:13.000000 incendium-stubs-2023.3.0/stubs/incendium/vision/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:28.325766 incendium-stubs-2023.3.0/stubs/incendium_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-03-30 23:56:28.000000 incendium-stubs-2023.3.0/stubs/incendium_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-03-30 23:56:28.000000 incendium-stubs-2023.3.0/stubs/incendium_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-30 23:56:28.000000 incendium-stubs-2023.3.0/stubs/incendium_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-03-30 23:56:28.000000 incendium-stubs-2023.3.0/stubs/incendium_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-03-30 23:56:28.000000 incendium-stubs-2023.3.0/stubs/incendium_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:27.009699 incendium-stubs-2023.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-04-19 00:28:27.009699 incendium-stubs-2023.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2040 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1575 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-19 00:28:27.009699 incendium-stubs-2023.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:26.997699 incendium-stubs-2023.4.0/stubs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:27.001699 incendium-stubs-2023.4.0/stubs/incendium/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      619 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      832 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/dataset.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/date.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2579 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/db.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      508 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/exceptions.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:27.005699 incendium-stubs-2023.4.0/stubs/incendium/helper/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/helper/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/helper/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      320 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/helper/types.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      395 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/net.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)      259 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/tag.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/user.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:27.005699 incendium-stubs-2023.4.0/stubs/incendium/vision/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/vision/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/vision/gui.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/vision/nav.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:10.000000 incendium-stubs-2023.4.0/stubs/incendium/vision/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:27.009699 incendium-stubs-2023.4.0/stubs/incendium_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     4648 2023-04-19 00:28:26.000000 incendium-stubs-2023.4.0/stubs/incendium_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-04-19 00:28:26.000000 incendium-stubs-2023.4.0/stubs/incendium_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 00:28:26.000000 incendium-stubs-2023.4.0/stubs/incendium_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-19 00:28:26.000000 incendium-stubs-2023.4.0/stubs/incendium_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-19 00:28:26.000000 incendium-stubs-2023.4.0/stubs/incendium_stubs.egg-info/top_level.txt
```

### Comparing `incendium-stubs-2023.3.0/LICENSE` & `incendium-stubs-2023.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `incendium-stubs-2023.3.0/PKG-INFO` & `incendium-stubs-2023.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incendium-stubs
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: incendium stubs package
 Author-email: César Román <cesar@thecesrom.dev>
 License: MIT License
         
         Copyright (c) 2022 César Román
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `incendium-stubs-2023.3.0/README.md` & `incendium-stubs-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `incendium-stubs-2023.3.0/pyproject.toml` & `incendium-stubs-2023.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "setuptools.build_meta"
 requires = [
   "setuptools>=61.2",
 ]
 
 [project]
 name = "incendium-stubs"
-version = "2023.3.0"
+version = "2023.4.0"
 description = "incendium stubs package"
 readme = "README.md"
 keywords = [
   "hmi",
   "ignition",
   "inductive automation",
   "scada",
```

### Comparing `incendium-stubs-2023.3.0/stubs/incendium/constants.pyi` & `incendium-stubs-2023.4.0/stubs/incendium/constants.pyi`

 * *Files identical despite different names*

### Comparing `incendium-stubs-2023.3.0/stubs/incendium/dataset.pyi` & `incendium-stubs-2023.4.0/stubs/incendium/dataset.pyi`

 * *Files identical despite different names*

### Comparing `incendium-stubs-2023.3.0/stubs/incendium/db.pyi` & `incendium-stubs-2023.4.0/stubs/incendium/db.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from types import TracebackType
 from typing import Any, List, Optional, Tuple, Type, Union
 
 from com.inductiveautomation.ignition.common import BasicDataset
 from incendium.helper.types import AnyStr, DictIntStringAny
 
 class DisposableConnection:
-    database: AnyStr
-    retries: int
     def __init__(self, database: AnyStr, retries: int = ...) -> None: ...
     @property
+    def database(self) -> AnyStr: ...
+    @property
     def status(self) -> AnyStr: ...
     def __enter__(self) -> DisposableConnection: ...
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
```

### Comparing `incendium-stubs-2023.3.0/stubs/incendium/user.pyi` & `incendium-stubs-2023.4.0/stubs/incendium/user.pyi`

 * *Files identical despite different names*

### Comparing `incendium-stubs-2023.3.0/stubs/incendium/util.pyi` & `incendium-stubs-2023.4.0/stubs/incendium/util.pyi`

 * *Files identical despite different names*

### Comparing `incendium-stubs-2023.3.0/stubs/incendium/vision/gui.pyi` & `incendium-stubs-2023.4.0/stubs/incendium/vision/gui.pyi`

 * *Files identical despite different names*

### Comparing `incendium-stubs-2023.3.0/stubs/incendium_stubs.egg-info/PKG-INFO` & `incendium-stubs-2023.4.0/stubs/incendium_stubs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incendium-stubs
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: incendium stubs package
 Author-email: César Román <cesar@thecesrom.dev>
 License: MIT License
         
         Copyright (c) 2022 César Román
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `incendium-stubs-2023.3.0/stubs/incendium_stubs.egg-info/SOURCES.txt` & `incendium-stubs-2023.4.0/stubs/incendium_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


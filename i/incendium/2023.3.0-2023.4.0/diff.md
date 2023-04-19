# Comparing `tmp/incendium-2023.3.0.tar.gz` & `tmp/incendium-2023.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/incendium/incendium/dist/tmpBucdUp/incendium-2023.3.0.tar", last modified: Thu Mar 30 23:56:23 2023, max compression
+gzip compressed data, was "/home/runner/work/incendium/incendium/dist/tmpn3HAbp/incendium-2023.4.0.tar", last modified: Wed Apr 19 00:28:20 2023, max compression
```

## Comparing `incendium-2023.3.0.tar` & `incendium-2023.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:23.000000 incendium-2023.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)    14182 2023-03-30 23:56:23.000000 incendium-2023.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4285 2023-03-30 23:56:11.000000 incendium-2023.3.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1423 2023-03-30 23:56:23.000000 incendium-2023.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-03-30 23:56:11.000000 incendium-2023.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-03-30 23:56:11.000000 incendium-2023.3.0/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:23.000000 incendium-2023.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:23.000000 incendium-2023.3.0/src/incendium/
--rw-r--r--   0 runner    (1001) docker     (122)    16659 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/db.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:23.000000 incendium-2023.3.0/src/incendium/helper/
--rw-r--r--   0 runner    (1001) docker     (122)      341 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/helper/types.py
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/user.py
--rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/date.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:23.000000 incendium-2023.3.0/src/incendium/vision/
--rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/vision/gui.py
--rw-r--r--   0 runner    (1001) docker     (122)      175 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/vision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/vision/nav.py
--rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      398 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/tag.py
--rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/net.py
--rw-r--r--   0 runner    (1001) docker     (122)     7468 2023-03-30 23:56:11.000000 incendium-2023.3.0/src/incendium/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-30 23:56:23.000000 incendium-2023.3.0/src/incendium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14182 2023-03-30 23:56:23.000000 incendium-2023.3.0/src/incendium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      646 2023-03-30 23:56:23.000000 incendium-2023.3.0/src/incendium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-03-30 23:56:23.000000 incendium-2023.3.0/src/incendium.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-03-30 23:56:23.000000 incendium-2023.3.0/src/incendium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-30 23:56:23.000000 incendium-2023.3.0/src/incendium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5529 2023-03-30 23:56:11.000000 incendium-2023.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-03-30 23:56:11.000000 incendium-2023.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       79 2023-03-30 23:56:11.000000 incendium-2023.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:20.000000 incendium-2023.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    14336 2023-04-19 00:28:20.000000 incendium-2023.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5529 2023-04-19 00:28:09.000000 incendium-2023.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-04-19 00:28:09.000000 incendium-2023.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14336 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      646 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium/
+-rw-r--r--   0 runner    (1001) docker     (122)      398 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium/vision/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/vision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10325 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/vision/gui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2735 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/vision/nav.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1292 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-19 00:28:20.000000 incendium-2023.4.0/src/incendium/helper/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      341 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/helper/types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6553 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/user.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/net.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1453 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/date.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7468 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3937 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17135 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/db.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2230 2023-04-19 00:28:09.000000 incendium-2023.4.0/src/incendium/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1430 2023-04-19 00:28:20.000000 incendium-2023.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1075 2023-04-19 00:28:09.000000 incendium-2023.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-04-19 00:28:09.000000 incendium-2023.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     4391 2023-04-19 00:28:09.000000 incendium-2023.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-04-19 00:28:09.000000 incendium-2023.4.0/setup.py
```

### Comparing `incendium-2023.3.0/PKG-INFO` & `incendium-2023.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incendium
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: Package that extends and wraps Ignition Scripting API
 Home-page: https://github.com/thecesrom/incendium
 Author: César Román
 Author-email: cesar@thecesrom.dev
 License: MIT
 Project-URL: Source, https://github.com/thecesrom/incendium
 Project-URL: Documentation, https://github.com/thecesrom/incendium/wiki
@@ -129,14 +129,20 @@
         
         See [LICENSE](./LICENSE).
         
         ## Code of conduct
         
         See [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md).
         
+        ## v2023.4.0 (2023-04-18)
+        
+        ### Feat
+        
+        - **db**: handle concurrent DisposableConnection connections (#142)
+        
         ## v2023.3.0 (2023-03-30)
         
         ### Feat
         
         - **dataset**: add from_list_of_dicts (#140)
         
         ### Refactor
```

### Comparing `incendium-2023.3.0/CHANGELOG.md` & `incendium-2023.4.0/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## v2023.4.0 (2023-04-18)
+
+### Feat
+
+- **db**: handle concurrent DisposableConnection connections (#142)
+
 ## v2023.3.0 (2023-03-30)
 
 ### Feat
 
 - **dataset**: add from_list_of_dicts (#140)
 
 ### Refactor
```

### Comparing `incendium-2023.3.0/setup.cfg` & `incendium-2023.4.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = incendium
-version = 2023.3.0
+version = 2023.4.0
 description = Package that extends and wraps Ignition Scripting API
 long_description = file: README.md, CHANGELOG.md
 long_description_content_type = text/markdown
 url = https://github.com/thecesrom/incendium
 author = César Román
 author_email = cesar@thecesrom.dev
 license = MIT
@@ -34,15 +34,15 @@
 	Funding = https://github.com/sponsors/thecesrom
 	Source = https://github.com/thecesrom/incendium
 	Tracker = https://github.com/thecesrom/incendium/issues
 
 [options]
 packages = find:
 install_requires = 
-	ignition-api
+	ignition-api>=8.1.0
 python_requires = ==2.7.18
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
```

### Comparing `incendium-2023.3.0/src/incendium/db.py` & `incendium-2023.4.0/src/incendium/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     "o_get_data",
 ]
 
 from types import TracebackType
 from typing import Any, List, Optional, Tuple, Type, TypedDict, Union
 
 import system.db
+import system.util
 from com.inductiveautomation.ignition.common import BasicDataset
 from java.lang import Thread
 
 from incendium.helper.types import AnyStr, DictIntStringAny
 
 _SProcResult = TypedDict(
     "_SProcResult",
@@ -38,75 +39,84 @@
     """Disposable Connection.
 
     A disposable connection enables a database connection in Ignition
     and disables it once the operation is completed to release
     resources.
     """
 
-    database = None  # type: AnyStr
-    retries = None  # type: int
-
     def __init__(self, database, retries=3):
         # type: (AnyStr, int) -> None
         """Disposable Connection initializer.
 
         Args:
             database: The name of the database connection in
                 Ignition.
             retries: The number of additional times to retry
                 enabling the connection. Optional.
         """
         super(DisposableConnection, self).__init__()
-        self.database = database
-        self.retries = retries
+        self._database = database
+        self._retries = retries
+        self._global_conn = "incendium_db_{}".format(database)
+
+    @property
+    def database(self):
+        # type: () -> AnyStr
+        """Get the name of the disposable connection."""
+        return self._database
 
     @property
     def status(self):
         # type: () -> AnyStr
         """Get connection status."""
-        connection_info = system.db.getConnectionInfo(self.database)
+        connection_info = system.db.getConnectionInfo(self._database)
         return str(connection_info.getValueAt(0, "Status"))
 
     def __enter__(self):
         # type: () -> DisposableConnection
         """Enter the runtime context related to this object.
 
         Raises:
             IOError: If the connection's status reports as Faulted, or
                 ir cannot be enabled.
         """
-        system.db.setDatasourceEnabled(self.database, True)
+        system.db.setDatasourceEnabled(self._database, True)
 
-        for _ in range(self.retries):
+        for _ in range(self._retries):
             Thread.sleep(1000)
             if self.status == "Valid":
+                if self._global_conn not in system.util.globals:
+                    system.util.globals[self._global_conn] = 0
+                system.util.globals[self._global_conn] += 1
                 break
             if self.status == "Faulted":
                 raise IOError(
                     "The database connection {!r} is {}.".format(
-                        self.database, self.status
+                        self._database, self.status
                     )
                 )
         else:
             raise IOError(
                 "The database connection {!r} could not be enabled.".format(
-                    self.database
+                    self._database
                 )
             )
         return self
 
     def __exit__(
         self,
         exc_type,  # type: Optional[Type[BaseException]]
         exc_val,  # type: Optional[BaseException]
         exc_tb,  # type: Optional[TracebackType]
     ):
         # type: (...) -> None
         """Exit the runtime context related to this object."""
-        system.db.setDatasourceEnabled(self.database, False)
+        system.util.globals[self._global_conn] -= 1
+        if system.util.globals[self._global_conn] == 0:
+            system.db.setDatasourceEnabled(self._database, False)
 
 
 class Param(object):
     """Base class used for defining [IN|OUT]PUT parameters."""
 
     def __init__(
         self,
```

### Comparing `incendium-2023.3.0/src/incendium/user.py` & `incendium-2023.4.0/src/incendium/user.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.3.0/src/incendium/date.py` & `incendium-2023.4.0/src/incendium/date.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.3.0/src/incendium/vision/gui.py` & `incendium-2023.4.0/src/incendium/vision/gui.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.3.0/src/incendium/vision/nav.py` & `incendium-2023.4.0/src/incendium/vision/nav.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.3.0/src/incendium/util.py` & `incendium-2023.4.0/src/incendium/util.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.3.0/src/incendium/constants.py` & `incendium-2023.4.0/src/incendium/constants.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.3.0/src/incendium/exceptions.py` & `incendium-2023.4.0/src/incendium/exceptions.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.3.0/src/incendium/tag.py` & `incendium-2023.4.0/src/incendium/tag.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.3.0/src/incendium/net.py` & `incendium-2023.4.0/src/incendium/net.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.3.0/src/incendium/dataset.py` & `incendium-2023.4.0/src/incendium/dataset.py`

 * *Files identical despite different names*

### Comparing `incendium-2023.3.0/src/incendium.egg-info/PKG-INFO` & `incendium-2023.4.0/src/incendium.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: incendium
-Version: 2023.3.0
+Version: 2023.4.0
 Summary: Package that extends and wraps Ignition Scripting API
 Home-page: https://github.com/thecesrom/incendium
 Author: César Román
 Author-email: cesar@thecesrom.dev
 License: MIT
 Project-URL: Source, https://github.com/thecesrom/incendium
 Project-URL: Documentation, https://github.com/thecesrom/incendium/wiki
@@ -129,14 +129,20 @@
         
         See [LICENSE](./LICENSE).
         
         ## Code of conduct
         
         See [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md).
         
+        ## v2023.4.0 (2023-04-18)
+        
+        ### Feat
+        
+        - **db**: handle concurrent DisposableConnection connections (#142)
+        
         ## v2023.3.0 (2023-03-30)
         
         ### Feat
         
         - **dataset**: add from_list_of_dicts (#140)
         
         ### Refactor
```

### Comparing `incendium-2023.3.0/src/incendium.egg-info/SOURCES.txt` & `incendium-2023.4.0/src/incendium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `incendium-2023.3.0/README.md` & `incendium-2023.4.0/README.md`

 * *Files identical despite different names*

### Comparing `incendium-2023.3.0/LICENSE` & `incendium-2023.4.0/LICENSE`

 * *Files identical despite different names*


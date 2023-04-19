# Comparing `tmp/Apppath-1.0.0.tar.gz` & `tmp/Apppath-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Apppath-1.0.0.tar", last modified: Thu Feb 16 14:32:46 2023, max compression
+gzip compressed data, was "Apppath-1.0.1.tar", last modified: Wed Apr 19 11:01:56 2023, max compression
```

## Comparing `Apppath-1.0.0.tar` & `Apppath-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:32:46.336007 Apppath-1.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:32:46.332007 Apppath-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-16 14:32:40.000000 Apppath-1.0.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:32:46.332007 Apppath-1.0.0/Apppath.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-02-16 14:32:46.000000 Apppath-1.0.0/Apppath.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-16 14:32:46.000000 Apppath-1.0.0/Apppath.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-16 14:32:46.000000 Apppath-1.0.0/Apppath.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-02-16 14:32:46.000000 Apppath-1.0.0/Apppath.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-02-16 14:32:46.000000 Apppath-1.0.0/Apppath.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-16 14:32:46.000000 Apppath-1.0.0/Apppath.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-16 14:32:40.000000 Apppath-1.0.0/KEYWORDS.md
--rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-02-16 14:32:40.000000 Apppath-1.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-16 14:32:40.000000 Apppath-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-02-16 14:32:46.336007 Apppath-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-02-16 14:32:40.000000 Apppath-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-02-16 14:32:40.000000 Apppath-1.0.0/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:32:46.336007 Apppath-1.0.0/apppath/
--rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-02-16 14:32:40.000000 Apppath-1.0.0/apppath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33765 2023-02-16 14:32:40.000000 Apppath-1.0.0/apppath/app_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:32:46.336007 Apppath-1.0.0/apppath/entry_points/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-16 14:32:40.000000 Apppath-1.0.0/apppath/entry_points/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-02-16 14:32:40.000000 Apppath-1.0.0/apppath/entry_points/clean_apppath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-16 14:32:40.000000 Apppath-1.0.0/apppath/entry_points/open_apppath.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-02-16 14:32:40.000000 Apppath-1.0.0/apppath/system_open_path_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-02-16 14:32:40.000000 Apppath-1.0.0/apppath/windows_path_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:32:46.336007 Apppath-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-02-16 14:32:40.000000 Apppath-1.0.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-02-16 14:32:40.000000 Apppath-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-16 14:32:40.000000 Apppath-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-16 14:32:46.336007 Apppath-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-02-16 14:32:40.000000 Apppath-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-16 14:32:46.336007 Apppath-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-02-16 14:32:40.000000 Apppath-1.0.0/tests/test_app_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-16 14:32:40.000000 Apppath-1.0.0/tests/test_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-16 14:32:40.000000 Apppath-1.0.0/tests/test_sanity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:51.000000 Apppath-1.0.1/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/Apppath.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-04-19 11:01:56.000000 Apppath-1.0.1/Apppath.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-19 11:01:56.000000 Apppath-1.0.1/Apppath.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:01:56.000000 Apppath-1.0.1/Apppath.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-04-19 11:01:56.000000 Apppath-1.0.1/Apppath.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-19 11:01:56.000000 Apppath-1.0.1/Apppath.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 11:01:56.000000 Apppath-1.0.1/Apppath.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-19 11:01:51.000000 Apppath-1.0.1/KEYWORDS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10644 2023-04-19 11:01:51.000000 Apppath-1.0.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-19 11:01:51.000000 Apppath-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-04-19 11:01:56.182758 Apppath-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-19 11:01:51.000000 Apppath-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-19 11:01:51.000000 Apppath-1.0.1/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/apppath/
+-rw-r--r--   0 runner    (1001) docker     (123)     3387 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34204 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/app_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/apppath/entry_points/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/entry_points/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/entry_points/clean_apppath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/entry_points/open_apppath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/system_open_path_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-04-19 11:01:51.000000 Apppath-1.0.1/apppath/windows_path_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-19 11:01:51.000000 Apppath-1.0.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-04-19 11:01:51.000000 Apppath-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-19 11:01:51.000000 Apppath-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-19 11:01:56.186758 Apppath-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-04-19 11:01:51.000000 Apppath-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:01:56.182758 Apppath-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-04-19 11:01:51.000000 Apppath-1.0.1/tests/test_app_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-19 11:01:51.000000 Apppath-1.0.1/tests/test_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-19 11:01:51.000000 Apppath-1.0.1/tests/test_sanity.py
```

### Comparing `Apppath-1.0.0/Apppath.egg-info/PKG-INFO` & `Apppath-1.0.1/Apppath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Apppath
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/apppath
 Download-URL: https://github.com/pything/apppath/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -19,18 +19,18 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: docs
-Provides-Extra: setup
+Provides-Extra: dev
 Provides-Extra: tests
+Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![apppath](.github/images/apppath.svg)-->
 
 <p align="center">
   <img src=".github/images/apppath.svg" alt='AppPath' />
```

### Comparing `Apppath-1.0.0/Apppath.egg-info/SOURCES.txt` & `Apppath-1.0.1/Apppath.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.0/LICENSE.md` & `Apppath-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.0/PKG-INFO` & `Apppath-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Apppath
-Version: 1.0.0
+Version: 1.0.1
 Summary: A package for easing return of multiple values
 Home-page: https://github.com/pything/apppath
 Download-URL: https://github.com/pything/apppath/releases
 Author: Christian Heider Nielsen
 Author-email: christian.heider@alexandra.dk
 Maintainer: Christian Heider Nielsen
 Maintainer-email: christian.heider@alexandra.dk
@@ -19,18 +19,18 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 Provides-Extra: docs
-Provides-Extra: setup
+Provides-Extra: dev
 Provides-Extra: tests
+Provides-Extra: setup
 Provides-Extra: all
 License-File: LICENSE.md
 
 <!--![apppath](.github/images/apppath.svg)-->
 
 <p align="center">
   <img src=".github/images/apppath.svg" alt='AppPath' />
```

### Comparing `Apppath-1.0.0/README.md` & `Apppath-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.0/SECURITY.md` & `Apppath-1.0.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.0/apppath/__init__.py` & `Apppath-1.0.1/apppath/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 from warnings import warn
 
 import pkg_resources
 
 __project__ = "Apppath"
 __author__ = "Christian Heider Nielsen"
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 __doc__ = r"""
 Created on 27/04/2019
 
 A class and a set of functions for providing for system-consensual path for apps to store data, logs, cache...
 
 @author: cnheider
 """
```

### Comparing `Apppath-1.0.0/apppath/app_path.py` & `Apppath-1.0.1/apppath/app_path.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,31 +82,46 @@
         :param app_name:
         :param app_author:
         :param app_version:
         :param roaming: "roaming" (boolean, default False) can be set True to use the Windows roaming appdata directory. That means that for users on a Windows network setup for roaming profiles, this user data will be sync'd on login. See <http://technet.microsoft.com/en-us/library/cc766489(WS.10).aspx> for a discussion of issues.
         :param multi_path: "multi_path" is an optional parameter only applicable to *nix which indicates that the entire list of data dirs should be returned. By default, the first item from XDG_DATA_DIRS is returned, or '/usr/local/share/<AppName>', if XDG_DATA_DIRS is not set
         :param ensure_existence_on_access:
         :param normalise_path:"""
-        assert isinstance(app_name, str)
+        assert isinstance(app_name, str), f"app_name must be a str, not {type(app_name)}"
 
         self._sanitise_path = normalise_path
+
         if normalise_path:
             app_name = app_name.strip().lower().replace(" ", "_")
+
         self._app_name = app_name
-        if isinstance(app_author, str):
-            if normalise_path:
-                app_author = app_author.strip().lower().replace(" ", "_")
-        else:
-            assert app_author is None
+
+        if app_author:
+            if isinstance(app_author, str):
+                if normalise_path:
+                    app_author = app_author.strip().lower().replace(" ", "_")
+            else:
+                assert (
+                    app_author is None
+                ), f"{type(app_author)} is not accepted as app_author, must be of type str or None"
+
         self._app_author = app_author
-        if isinstance(app_version, (int, float)):
-            app_version = str(app_version)
-        if isinstance(app_version, str):
-            if normalise_path:
-                app_version = app_version.strip().lower().replace(" ", "_")
+
+        if app_version:
+            if isinstance(app_version, (int, float)):
+                app_version = str(app_version)
+
+            if isinstance(app_version, str):
+                if normalise_path:
+                    app_version = app_version.strip().lower().replace(" ", "_")
+            else:
+                raise TypeError(
+                    f"app_version was of type {type(app_version)}, only int, float and str is supported"
+                )
+
         self._app_version = app_version
         self._roaming = roaming
         self._multi_path = multi_path
         self._ensure_existence = ensure_existence_on_access
 
     def __divmod__(self, other):
         return self.__truediv__(other)
```

### Comparing `Apppath-1.0.0/apppath/entry_points/clean_apppath.py` & `Apppath-1.0.1/apppath/entry_points/clean_apppath.py`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.0/apppath/entry_points/open_apppath.py` & `Apppath-1.0.1/apppath/entry_points/open_apppath.py`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.0/apppath/system_open_path_utilities.py` & `Apppath-1.0.1/apppath/system_open_path_utilities.py`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.0/apppath/windows_path_utilities.py` & `Apppath-1.0.1/apppath/windows_path_utilities.py`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.0/pyproject.toml` & `Apppath-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.0/setup.py` & `Apppath-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `Apppath-1.0.0/tests/test_app_path.py` & `Apppath-1.0.1/tests/test_app_path.py`

 * *Files identical despite different names*


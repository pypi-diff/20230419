# Comparing `tmp/veritas-0.1.8.tar.gz` & `tmp/veritas-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veritas-0.1.8.tar", last modified: Mon Jan 16 08:43:29 2023, max compression
+gzip compressed data, was "veritas-0.1.9.tar", last modified: Mon Jan 16 08:57:47 2023, max compression
```

## Comparing `veritas-0.1.8.tar` & `veritas-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lonnen     (501) staff       (20)        0 2023-01-16 08:43:29.412824 veritas-0.1.8/
--rw-r--r--   0 lonnen     (501) staff       (20)     1488 2023-01-16 08:36:11.000000 veritas-0.1.8/LICENSE
--rw-r--r--   0 lonnen     (501) staff       (20)     1697 2023-01-16 08:43:29.412536 veritas-0.1.8/PKG-INFO
--rw-r--r--   0 lonnen     (501) staff       (20)     1013 2023-01-16 08:39:03.000000 veritas-0.1.8/README.rst
--rw-r--r--   0 lonnen     (501) staff       (20)       38 2023-01-16 08:43:29.412911 veritas-0.1.8/setup.cfg
--rw-r--r--   0 lonnen     (501) staff       (20)     1155 2023-01-16 08:37:56.000000 veritas-0.1.8/setup.py
-drwxr-xr-x   0 lonnen     (501) staff       (20)        0 2023-01-16 08:43:29.410583 veritas-0.1.8/tests/
--rw-r--r--   0 lonnen     (501) staff       (20)        0 2020-04-23 04:04:55.000000 veritas-0.1.8/tests/__init__.py
--rw-r--r--   0 lonnen     (501) staff       (20)     4473 2020-04-23 16:13:59.000000 veritas-0.1.8/tests/test_veritas.py
-drwxr-xr-x   0 lonnen     (501) staff       (20)        0 2023-01-16 08:43:29.410966 veritas-0.1.8/veritas/
--rw-r--r--   0 lonnen     (501) staff       (20)     2920 2023-01-16 08:40:30.000000 veritas-0.1.8/veritas/__init__.py
-drwxr-xr-x   0 lonnen     (501) staff       (20)        0 2023-01-16 08:43:29.412230 veritas-0.1.8/veritas.egg-info/
--rw-r--r--   0 lonnen     (501) staff       (20)     1697 2023-01-16 08:43:29.000000 veritas-0.1.8/veritas.egg-info/PKG-INFO
--rw-r--r--   0 lonnen     (501) staff       (20)      211 2023-01-16 08:43:29.000000 veritas-0.1.8/veritas.egg-info/SOURCES.txt
--rw-r--r--   0 lonnen     (501) staff       (20)        1 2023-01-16 08:43:29.000000 veritas-0.1.8/veritas.egg-info/dependency_links.txt
--rw-r--r--   0 lonnen     (501) staff       (20)       14 2023-01-16 08:43:29.000000 veritas-0.1.8/veritas.egg-info/top_level.txt
+drwxr-xr-x   0 lonnen     (501) staff       (20)        0 2023-01-16 08:57:47.256909 veritas-0.1.9/
+-rw-r--r--   0 lonnen     (501) staff       (20)     1488 2023-01-16 08:36:11.000000 veritas-0.1.9/LICENSE
+-rw-r--r--   0 lonnen     (501) staff       (20)     2013 2023-01-16 08:57:47.256636 veritas-0.1.9/PKG-INFO
+-rw-r--r--   0 lonnen     (501) staff       (20)     1329 2023-01-16 08:54:12.000000 veritas-0.1.9/README.rst
+-rw-r--r--   0 lonnen     (501) staff       (20)       38 2023-01-16 08:57:47.256988 veritas-0.1.9/setup.cfg
+-rw-r--r--   0 lonnen     (501) staff       (20)     1155 2023-01-16 08:37:56.000000 veritas-0.1.9/setup.py
+drwxr-xr-x   0 lonnen     (501) staff       (20)        0 2023-01-16 08:57:47.254822 veritas-0.1.9/tests/
+-rw-r--r--   0 lonnen     (501) staff       (20)        0 2020-04-23 04:04:55.000000 veritas-0.1.9/tests/__init__.py
+-rw-r--r--   0 lonnen     (501) staff       (20)     4473 2020-04-23 16:13:59.000000 veritas-0.1.9/tests/test_veritas.py
+drwxr-xr-x   0 lonnen     (501) staff       (20)        0 2023-01-16 08:57:47.255091 veritas-0.1.9/veritas/
+-rw-r--r--   0 lonnen     (501) staff       (20)     2920 2023-01-16 08:54:43.000000 veritas-0.1.9/veritas/__init__.py
+drwxr-xr-x   0 lonnen     (501) staff       (20)        0 2023-01-16 08:57:47.256306 veritas-0.1.9/veritas.egg-info/
+-rw-r--r--   0 lonnen     (501) staff       (20)     2013 2023-01-16 08:57:47.000000 veritas-0.1.9/veritas.egg-info/PKG-INFO
+-rw-r--r--   0 lonnen     (501) staff       (20)      211 2023-01-16 08:57:47.000000 veritas-0.1.9/veritas.egg-info/SOURCES.txt
+-rw-r--r--   0 lonnen     (501) staff       (20)        1 2023-01-16 08:57:47.000000 veritas-0.1.9/veritas.egg-info/dependency_links.txt
+-rw-r--r--   0 lonnen     (501) staff       (20)       14 2023-01-16 08:57:47.000000 veritas-0.1.9/veritas.egg-info/top_level.txt
```

### Comparing `veritas-0.1.8/LICENSE` & `veritas-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `veritas-0.1.8/PKG-INFO` & `veritas-0.1.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veritas
-Version: 0.1.8
+Version: 0.1.9
 Summary: an executable implementation of the throwaway `_`
 Home-page: https://github.com/lonnen/veritas
 Author: lonnen
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -20,17 +20,21 @@
 veritas
 =======
 
 Veritas is a Python library implementing a throwaway variable that attempts to return true no matter how it is called upon.
 
 It is intended for writing tests where you must provide some variables to an interface but your particular test will never read what happens to them. Veritas attempts to make sure that whatever the side effects on these variables it will not derail program execution. It implements comparable, numeric, callable, container, iterator, binary, in-place, unary, context manager, and async interfaces.
 
+Needing this is a smell, but it can help you get things moving without requiring you to refactor the whole system.
+
+[![CI](https://github.com/lonnen/veritas/actions/workflows/main.yml/badge.svg)](https://github.com/lonnen/veritas/actions/workflows/main.yml)
 
 :Code:          https://github.com/lonnen/veritas/
 :Issues:        https://github.com/lonnen/veritas/issues
+:Releases:      https://pypi.org/project/veritas/#history
 :License:       BSD 3-clause; See LICENSE
 
 Install
 =======
 
 From PyPI
 ---------
```

### Comparing `veritas-0.1.8/README.rst` & `veritas-0.1.9/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 veritas
 =======
 
 Veritas is a Python library implementing a throwaway variable that attempts to return true no matter how it is called upon.
 
 It is intended for writing tests where you must provide some variables to an interface but your particular test will never read what happens to them. Veritas attempts to make sure that whatever the side effects on these variables it will not derail program execution. It implements comparable, numeric, callable, container, iterator, binary, in-place, unary, context manager, and async interfaces.
 
+Needing this is a smell, but it can help you get things moving without requiring you to refactor the whole system.
+
+[![CI](https://github.com/lonnen/veritas/actions/workflows/main.yml/badge.svg)](https://github.com/lonnen/veritas/actions/workflows/main.yml)
 
 :Code:          https://github.com/lonnen/veritas/
 :Issues:        https://github.com/lonnen/veritas/issues
+:Releases:      https://pypi.org/project/veritas/#history
 :License:       BSD 3-clause; See LICENSE
 
 Install
 =======
 
 From PyPI
 ---------
```

### Comparing `veritas-0.1.8/setup.py` & `veritas-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `veritas-0.1.8/tests/test_veritas.py` & `veritas-0.1.9/tests/test_veritas.py`

 * *Files identical despite different names*

### Comparing `veritas-0.1.8/veritas/__init__.py` & `veritas-0.1.9/veritas/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 
 class Veritas(object):
     """An executable implementation of _ in function definitions.
 
     Attempts to implement all generic interfaces and, when possible,
     always evaluate to True. Inspired by mock._ANY and
```

### Comparing `veritas-0.1.8/veritas.egg-info/PKG-INFO` & `veritas-0.1.9/veritas.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veritas
-Version: 0.1.8
+Version: 0.1.9
 Summary: an executable implementation of the throwaway `_`
 Home-page: https://github.com/lonnen/veritas
 Author: lonnen
 License: BSD
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -20,17 +20,21 @@
 veritas
 =======
 
 Veritas is a Python library implementing a throwaway variable that attempts to return true no matter how it is called upon.
 
 It is intended for writing tests where you must provide some variables to an interface but your particular test will never read what happens to them. Veritas attempts to make sure that whatever the side effects on these variables it will not derail program execution. It implements comparable, numeric, callable, container, iterator, binary, in-place, unary, context manager, and async interfaces.
 
+Needing this is a smell, but it can help you get things moving without requiring you to refactor the whole system.
+
+[![CI](https://github.com/lonnen/veritas/actions/workflows/main.yml/badge.svg)](https://github.com/lonnen/veritas/actions/workflows/main.yml)
 
 :Code:          https://github.com/lonnen/veritas/
 :Issues:        https://github.com/lonnen/veritas/issues
+:Releases:      https://pypi.org/project/veritas/#history
 :License:       BSD 3-clause; See LICENSE
 
 Install
 =======
 
 From PyPI
 ---------
```


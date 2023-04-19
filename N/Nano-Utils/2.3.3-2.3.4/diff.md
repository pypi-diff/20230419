# Comparing `tmp/Nano-Utils-2.3.3.tar.gz` & `tmp/Nano-Utils-2.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Nano-Utils-2.3.3.tar", last modified: Wed Jun 15 14:58:18 2022, max compression
+gzip compressed data, was "Nano-Utils-2.3.4.tar", last modified: Wed Apr 19 15:39:10 2023, max compression
```

## Comparing `Nano-Utils-2.3.3.tar` & `Nano-Utils-2.3.4.tar`

### file list

```diff
@@ -1,36 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:58:18.306197 Nano-Utils-2.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)       51 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:58:18.306197 Nano-Utils-2.3.3/Nano_Utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2529 2022-06-15 14:58:18.000000 Nano-Utils-2.3.3/Nano_Utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      732 2022-06-15 14:58:18.000000 Nano-Utils-2.3.3/Nano_Utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-15 14:58:18.000000 Nano-Utils-2.3.3/Nano_Utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-15 14:58:18.000000 Nano-Utils-2.3.3/Nano_Utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-06-15 14:58:18.000000 Nano-Utils-2.3.3/Nano_Utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-06-15 14:58:18.000000 Nano-Utils-2.3.3/Nano_Utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2529 2022-06-15 14:58:18.306197 Nano-Utils-2.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-15 14:58:18.306197 Nano-Utils-2.3.3/nanoutils/
--rw-r--r--   0 runner    (1001) docker     (121)      987 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3834 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/_catch_err.py
--rw-r--r--   0 runner    (1001) docker     (121)    11379 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/_dtype_mapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     8597 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/_lazy_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/_partial.py
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/_partial.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     6842 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/_seq_view.py
--rw-r--r--   0 runner    (1001) docker     (121)     4790 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/_set_attr.py
--rw-r--r--   0 runner    (1001) docker     (121)    10854 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/_user_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     1857 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/empty.py
--rw-r--r--   0 runner    (1001) docker     (121)    11675 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/file_container.py
--rw-r--r--   0 runner    (1001) docker     (121)    13060 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/hdf5_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6730 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)    12550 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/testing_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4610 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/typing_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    24665 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2671 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/nanoutils/yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      550 2022-06-15 14:58:18.306197 Nano-Utils-2.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2699 2022-06-15 14:57:52.000000 Nano-Utils-2.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:39:10.325431 Nano-Utils-2.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:39:10.321431 Nano-Utils-2.3.4/Nano_Utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-19 15:39:10.000000 Nano-Utils-2.3.4/Nano_Utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-19 15:39:10.000000 Nano-Utils-2.3.4/Nano_Utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:39:10.000000 Nano-Utils-2.3.4/Nano_Utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 15:39:10.000000 Nano-Utils-2.3.4/Nano_Utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-19 15:39:10.000000 Nano-Utils-2.3.4/Nano_Utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-19 15:39:10.000000 Nano-Utils-2.3.4/Nano_Utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-19 15:39:10.325431 Nano-Utils-2.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:39:10.325431 Nano-Utils-2.3.4/nanoutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/_catch_err.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11379 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/_dtype_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/_lazy_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/_partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/_partial.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6842 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/_seq_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/_set_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/_user_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11675 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/file_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13060 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/hdf5_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12524 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/typing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24665 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/nanoutils/yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-19 15:39:10.325431 Nano-Utils-2.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 15:39:10.325431 Nano-Utils-2.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/tests/test_dtype_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/tests/test_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/tests/test_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/tests/test_lazy_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/tests/test_sequence_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/tests/test_set_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/tests/test_sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/tests/test_testing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/tests/test_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/tests/test_user_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-04-19 15:38:48.000000 Nano-Utils-2.3.4/tests/test_utils.py
```

### Comparing `Nano-Utils-2.3.3/LICENSE.md` & `Nano-Utils-2.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/Nano_Utils.egg-info/PKG-INFO` & `Nano-Utils-2.3.4/Nano_Utils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: Nano-Utils
-Version: 2.3.3
+Version: 2.3.4
 Summary: Utility functions used throughout the various nlesc-nano repositories.
 Home-page: https://github.com/nlesc-nano/Nano-Utils
-Author: ['Bas van Beek']
+Author: Bas van Beek
 Author-email: b.f.van.beek@vu.nl
 License: Apache Software License
-Keywords: python-3,python-3-7,python-3-8,python-3-9,libraries
-Platform: UNKNOWN
+Keywords: python-3,python-3-7,python-3-8,python-3-9,python-3-10,python-3-11,libraries
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: test_no_optional
@@ -47,23 +47,22 @@
     :target: https://docs.python.org/3.7/
 .. image:: https://img.shields.io/badge/python-3.8-blue.svg
     :target: https://docs.python.org/3.8/
 .. image:: https://img.shields.io/badge/python-3.9-blue.svg
     :target: https://docs.python.org/3.9/
 .. image:: https://img.shields.io/badge/python-3.10-blue.svg
     :target: https://docs.python.org/3.10/
+.. image:: https://img.shields.io/badge/python-3.11-blue.svg
+    :target: https://docs.python.org/3.11/
 
-
-################
-Nano-Utils 2.3.3
-################
+##########
+Nano-Utils
+##########
 Utility functions used throughout the various nlesc-nano repositories.
 
 
 Installation
 ************
 * PyPi: ``pip install Nano-Utils``
 * GitHub: ``pip install git+https://github.com/nlesc-nano/Nano-Utils@master``
 
 
-
-
```

### Comparing `Nano-Utils-2.3.3/Nano_Utils.egg-info/SOURCES.txt` & `Nano-Utils-2.3.4/Nano_Utils.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE.md
 MANIFEST.in
 NOTICE
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 Nano_Utils.egg-info/PKG-INFO
 Nano_Utils.egg-info/SOURCES.txt
 Nano_Utils.egg-info/dependency_links.txt
 Nano_Utils.egg-info/not-zip-safe
 Nano_Utils.egg-info/requires.txt
@@ -25,8 +26,20 @@
 nanoutils/hdf5_utils.py
 nanoutils/numpy_utils.py
 nanoutils/py.typed
 nanoutils/schema.py
 nanoutils/testing_utils.py
 nanoutils/typing_utils.py
 nanoutils/utils.py
-nanoutils/yaml_utils.py
+nanoutils/yaml_utils.py
+tests/test_build.py
+tests/test_dtype_mapping.py
+tests/test_empty.py
+tests/test_hdf5.py
+tests/test_lazy_import.py
+tests/test_sequence_view.py
+tests/test_set_attr.py
+tests/test_sphinx.py
+tests/test_testing_utils.py
+tests/test_typing.py
+tests/test_user_mapping.py
+tests/test_utils.py
```

### Comparing `Nano-Utils-2.3.3/PKG-INFO` & `Nano-Utils-2.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: Nano-Utils
-Version: 2.3.3
+Version: 2.3.4
 Summary: Utility functions used throughout the various nlesc-nano repositories.
 Home-page: https://github.com/nlesc-nano/Nano-Utils
-Author: ['Bas van Beek']
+Author: Bas van Beek
 Author-email: b.f.van.beek@vu.nl
 License: Apache Software License
-Keywords: python-3,python-3-7,python-3-8,python-3-9,libraries
-Platform: UNKNOWN
+Keywords: python-3,python-3-7,python-3-8,python-3-9,python-3-10,python-3-11,libraries
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: doc
 Provides-Extra: test
 Provides-Extra: test_no_optional
@@ -47,23 +47,22 @@
     :target: https://docs.python.org/3.7/
 .. image:: https://img.shields.io/badge/python-3.8-blue.svg
     :target: https://docs.python.org/3.8/
 .. image:: https://img.shields.io/badge/python-3.9-blue.svg
     :target: https://docs.python.org/3.9/
 .. image:: https://img.shields.io/badge/python-3.10-blue.svg
     :target: https://docs.python.org/3.10/
+.. image:: https://img.shields.io/badge/python-3.11-blue.svg
+    :target: https://docs.python.org/3.11/
 
-
-################
-Nano-Utils 2.3.3
-################
+##########
+Nano-Utils
+##########
 Utility functions used throughout the various nlesc-nano repositories.
 
 
 Installation
 ************
 * PyPi: ``pip install Nano-Utils``
 * GitHub: ``pip install git+https://github.com/nlesc-nano/Nano-Utils@master``
 
 
-
-
```

### Comparing `Nano-Utils-2.3.3/README.rst` & `Nano-Utils-2.3.4/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -15,19 +15,20 @@
     :target: https://docs.python.org/3.7/
 .. image:: https://img.shields.io/badge/python-3.8-blue.svg
     :target: https://docs.python.org/3.8/
 .. image:: https://img.shields.io/badge/python-3.9-blue.svg
     :target: https://docs.python.org/3.9/
 .. image:: https://img.shields.io/badge/python-3.10-blue.svg
     :target: https://docs.python.org/3.10/
+.. image:: https://img.shields.io/badge/python-3.11-blue.svg
+    :target: https://docs.python.org/3.11/
 
-
-################
-Nano-Utils 2.3.3
-################
+##########
+Nano-Utils
+##########
 Utility functions used throughout the various nlesc-nano repositories.
 
 
 Installation
 ************
 * PyPi: ``pip install Nano-Utils``
 * GitHub: ``pip install git+https://github.com/nlesc-nano/Nano-Utils@master``
```

### Comparing `Nano-Utils-2.3.3/nanoutils/__init__.py` & `Nano-Utils-2.3.4/nanoutils/__init__.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/_catch_err.py` & `Nano-Utils-2.3.4/nanoutils/_catch_err.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/_dtype_mapping.py` & `Nano-Utils-2.3.4/nanoutils/_dtype_mapping.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/_lazy_import.py` & `Nano-Utils-2.3.4/nanoutils/_lazy_import.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/_partial.py` & `Nano-Utils-2.3.4/nanoutils/_partial.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/_seq_view.py` & `Nano-Utils-2.3.4/nanoutils/_seq_view.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/_set_attr.py` & `Nano-Utils-2.3.4/nanoutils/_set_attr.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/_user_dict.py` & `Nano-Utils-2.3.4/nanoutils/_user_dict.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/empty.py` & `Nano-Utils-2.3.4/nanoutils/empty.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/file_container.py` & `Nano-Utils-2.3.4/nanoutils/file_container.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/hdf5_utils.py` & `Nano-Utils-2.3.4/nanoutils/hdf5_utils.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/numpy_utils.py` & `Nano-Utils-2.3.4/nanoutils/numpy_utils.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/schema.py` & `Nano-Utils-2.3.4/nanoutils/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         except Exception as ex:
             err = RuntimeWarning(ex)
             err.__cause__ = ex
             warnings.warn(err)
             return repr(obj)
 
     @property
-    def __mod__(self) -> Callable[[object], str]:  # type: ignore[override]
+    def __mod__(self) -> Callable[[object], str]:
         """Get :meth:`Formatter.format`."""
         return self.format
 
 
 _PO = inspect.Parameter.POSITIONAL_ONLY
 _POK = inspect.Parameter.POSITIONAL_OR_KEYWORD
```

### Comparing `Nano-Utils-2.3.3/nanoutils/testing_utils.py` & `Nano-Utils-2.3.4/nanoutils/testing_utils.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/typing_utils.py` & `Nano-Utils-2.3.4/nanoutils/typing_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,16 +63,18 @@
 if sys.version_info < (3, 8):
     from typing_extensions import Literal, Final, final, Protocol, TypedDict, runtime_checkable, SupportsIndex  # noqa: E501
 else:
     from typing import Literal, Final, final, Protocol, TypedDict, SupportsIndex, runtime_checkable
 
 if TYPE_CHECKING:
     # Requires numpy >= 1.20
-    from numpy.typing import ArrayLike, DTypeLike, _ShapeLike as ShapeLike
+    from numpy.typing import ArrayLike, DTypeLike
     from numpy.typing import DTypeLike as DtypeLike
+    from typing import Sequence
+    ShapeLike = Union[SupportsIndex, Sequence[SupportsIndex]]
 
 else:
     ArrayLike = 'numpy.typing.ArrayLike'
     DTypeLike = 'numpy.typing.DTypeLike'
     DtypeLike = DTypeLike
     ShapeLike = 'numpy.typing._ShapeLike'
```

### Comparing `Nano-Utils-2.3.3/nanoutils/utils.py` & `Nano-Utils-2.3.4/nanoutils/utils.py`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/nanoutils/yaml_utils.py` & `Nano-Utils-2.3.4/nanoutils/yaml_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 from .utils import raise_if
 
 try:
     import yaml
     try:
         from yaml import CLoader as Loader
     except ImportError:
-        from yaml import Loader  # type: ignore[misc]
+        from yaml import Loader  # type: ignore[assignment]
     YAML_EX: None | Exception = None
 except Exception as ex:
-    from builtins import object as Loader  # type: ignore[misc]
+    from builtins import object as Loader  # type: ignore[assignment]
     YAML_EX = ex
 
 __all__ = ['UniqueLoader']
 
 
 class UniqueLoader(Loader):
     '''A :class:`yaml.Loader` subclass that dissallows for duplicate keys.
```

### Comparing `Nano-Utils-2.3.3/setup.cfg` & `Nano-Utils-2.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `Nano-Utils-2.3.3/setup.py` & `Nano-Utils-2.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,42 +46,45 @@
 
 setup(
     name='Nano-Utils',
     version=version['__version__'],
     description='Utility functions used throughout the various nlesc-nano repositories.',
     long_description=f'{readme}\n\n',
     long_description_content_type='text/x-rst',
-    author=['Bas van Beek'],
+    author='Bas van Beek',
     author_email='b.f.van.beek@vu.nl',
     url='https://github.com/nlesc-nano/Nano-Utils',
     packages=['nanoutils'],
     package_dir={'nanoutils': 'nanoutils'},
     package_data={'nanoutils': ['py.typed', '*.pyi']},
     include_package_data=True,
     license='Apache Software License',
     zip_safe=False,
     keywords=[
         'python-3',
         'python-3-7',
         'python-3-8',
         'python-3-9',
+        'python-3-10',
+        'python-3-11',
         'libraries'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development :: Libraries',
         'Typing :: Typed'
     ],
     python_requires='>=3.7',
     install_requires=[
         'typing_extensions>=3.10.0; python_version<"3.8"',
     ],
```


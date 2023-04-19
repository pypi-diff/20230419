# Comparing `tmp/Dickens-2.1.0.tar.gz` & `tmp/Dickens-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Dickens-2.1.0.tar", last modified: Tue Apr 11 19:11:25 2023, max compression
+gzip compressed data, was "Dickens-2.1.1.tar", last modified: Wed Apr 19 19:53:11 2023, max compression
```

## Comparing `Dickens-2.1.0.tar` & `Dickens-2.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-11 19:11:25.967497 Dickens-2.1.0/
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     3164 2023-04-11 19:11:25.967497 Dickens-2.1.0/PKG-INFO
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     1920 2022-07-19 19:31:17.140223 Dickens-2.1.0/README.rst
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     1150 2022-07-19 19:25:45.032469 Dickens-2.1.0/setup.py
-drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-11 19:11:25.967497 Dickens-2.1.0/src/
--rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     4985 2023-04-11 18:53:33.163336 Dickens-2.1.0/src/descriptors.py
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-19 19:53:11.755861 Dickens-2.1.1/
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     3164 2023-04-19 19:53:11.755861 Dickens-2.1.1/PKG-INFO
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     1920 2022-07-19 19:31:17.140223 Dickens-2.1.1/README.rst
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     1150 2022-07-19 19:25:45.032469 Dickens-2.1.1/setup.py
+drwxrwxr-x   0 jslondon  (1000) jslondon  (1000)        0 2023-04-19 19:53:11.755861 Dickens-2.1.1/src/
+-rw-rw-r--   0 jslondon  (1000) jslondon  (1000)     5072 2023-04-19 19:52:25.024158 Dickens-2.1.1/src/descriptors.py
```

### Comparing `Dickens-2.1.0/PKG-INFO` & `Dickens-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Dickens
-Version: 2.1.0
+Version: 2.1.1
 Summary: Additional decorators implementing the descriptor interface
 Home-page: https://github.com/dssg/dickens
 Author: Center for Data Science and Public Policy
 Author-email: datascifellows@gmail.com
 License: UNKNOWN
 Description: =======
         Dickens
```

### Comparing `Dickens-2.1.0/README.rst` & `Dickens-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `Dickens-2.1.0/setup.py` & `Dickens-2.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `Dickens-2.1.0/src/descriptors.py` & `Dickens-2.1.1/src/descriptors.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Additional decorators implementing the descriptor interface.
 
 """
 import functools
 import types
 
 
-__version__ = '2.1.0'
+__version__ = '2.1.1'
 
 
 class classproperty:
     """Descriptor decorator implementing a class-level read-only
     property.
 
     """
@@ -170,8 +170,11 @@
             raise TypeError(
                 f"'__dict__' of instance of type {instance.__class__.__name__} does "
                 f"not support item assignment for cache of property {self.__name__}"
             ) from None
 
         return value
 
-    __class_getitem__ = classmethod(types.GenericAlias)
+
+# Conditional to support Python 3.8
+if hasattr(types, 'GenericAlias'):
+    cachedproperty.__class_getitem__ = classmethod(types.GenericAlias)
```


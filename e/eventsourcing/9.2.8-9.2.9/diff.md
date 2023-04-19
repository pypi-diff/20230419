# Comparing `tmp/eventsourcing-9.2.8.tar.gz` & `tmp/eventsourcing-9.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eventsourcing-9.2.8.tar", last modified: Thu Apr 21 15:51:18 2022, max compression
+gzip compressed data, was "dist/eventsourcing-9.2.9.tar", last modified: Sat Apr 23 16:56:20 2022, max compression
```

## Comparing `eventsourcing-9.2.8.tar` & `eventsourcing-9.2.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-04-21 15:51:18.000000 eventsourcing-9.2.8/
--rw-r--r--   0 john       (501) staff       (20)      137 2022-03-17 22:05:19.000000 eventsourcing-9.2.8/AUTHORS
--rw-r--r--   0 john       (501) staff       (20)     1512 2022-03-17 22:05:19.000000 eventsourcing-9.2.8/LICENSE
--rw-r--r--   0 john       (501) staff       (20)     9017 2022-04-21 15:51:18.000000 eventsourcing-9.2.8/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)     7471 2022-03-17 22:05:19.000000 eventsourcing-9.2.8/README.md
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-04-21 15:51:18.000000 eventsourcing-9.2.8/eventsourcing/
--rw-r--r--   0 john       (501) staff       (20)       22 2022-04-21 15:34:36.000000 eventsourcing-9.2.8/eventsourcing/__init__.py
--rw-r--r--   0 john       (501) staff       (20)    36097 2022-04-20 16:25:50.000000 eventsourcing-9.2.8/eventsourcing/application.py
--rw-r--r--   0 john       (501) staff       (20)     3093 2022-04-20 16:25:25.000000 eventsourcing-9.2.8/eventsourcing/cipher.py
--rw-r--r--   0 john       (501) staff       (20)      385 2022-03-17 22:05:19.000000 eventsourcing-9.2.8/eventsourcing/compressor.py
--rw-r--r--   0 john       (501) staff       (20)     1489 2022-04-20 16:25:50.000000 eventsourcing-9.2.8/eventsourcing/dispatch.py
--rw-r--r--   0 john       (501) staff       (20)    51953 2022-04-21 14:42:20.000000 eventsourcing-9.2.8/eventsourcing/domain.py
--rw-r--r--   0 john       (501) staff       (20)     4653 2022-03-17 22:05:19.000000 eventsourcing-9.2.8/eventsourcing/interface.py
--rw-r--r--   0 john       (501) staff       (20)    37426 2022-04-20 16:25:50.000000 eventsourcing-9.2.8/eventsourcing/persistence.py
--rw-r--r--   0 john       (501) staff       (20)     6485 2022-03-17 22:05:19.000000 eventsourcing-9.2.8/eventsourcing/popo.py
--rw-r--r--   0 john       (501) staff       (20)    36635 2022-04-20 16:25:25.000000 eventsourcing-9.2.8/eventsourcing/postgres.py
--rw-r--r--   0 john       (501) staff       (20)        0 2022-03-15 14:47:08.000000 eventsourcing-9.2.8/eventsourcing/py.typed
--rw-r--r--   0 john       (501) staff       (20)    18860 2022-04-20 16:25:25.000000 eventsourcing-9.2.8/eventsourcing/sqlite.py
--rw-r--r--   0 john       (501) staff       (20)    45604 2022-04-21 14:43:50.000000 eventsourcing-9.2.8/eventsourcing/system.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-04-21 15:51:18.000000 eventsourcing-9.2.8/eventsourcing/tests/
--rw-r--r--   0 john       (501) staff       (20)        0 2021-11-19 02:39:53.000000 eventsourcing-9.2.8/eventsourcing/tests/__init__.py
--rw-r--r--   0 john       (501) staff       (20)    17022 2022-04-20 16:25:25.000000 eventsourcing-9.2.8/eventsourcing/tests/application.py
--rw-r--r--   0 john       (501) staff       (20)     3256 2022-04-20 16:25:25.000000 eventsourcing-9.2.8/eventsourcing/tests/domain.py
--rw-r--r--   0 john       (501) staff       (20)    43485 2022-04-20 16:25:25.000000 eventsourcing-9.2.8/eventsourcing/tests/persistence.py
--rw-r--r--   0 john       (501) staff       (20)     1340 2022-03-17 22:05:20.000000 eventsourcing-9.2.8/eventsourcing/tests/postgres_utils.py
--rw-r--r--   0 john       (501) staff       (20)     8451 2022-04-20 16:25:50.000000 eventsourcing-9.2.8/eventsourcing/utils.py
-drwxr-xr-x   0 john       (501) staff       (20)        0 2022-04-21 15:51:18.000000 eventsourcing-9.2.8/eventsourcing.egg-info/
--rw-r--r--   0 john       (501) staff       (20)     9017 2022-04-21 15:51:17.000000 eventsourcing-9.2.8/eventsourcing.egg-info/PKG-INFO
--rw-r--r--   0 john       (501) staff       (20)      789 2022-04-21 15:51:17.000000 eventsourcing-9.2.8/eventsourcing.egg-info/SOURCES.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2022-04-21 15:51:17.000000 eventsourcing-9.2.8/eventsourcing.egg-info/dependency_links.txt
--rw-r--r--   0 john       (501) staff       (20)        1 2021-12-15 16:43:28.000000 eventsourcing-9.2.8/eventsourcing.egg-info/not-zip-safe
--rw-r--r--   0 john       (501) staff       (20)      480 2022-04-21 15:51:17.000000 eventsourcing-9.2.8/eventsourcing.egg-info/requires.txt
--rw-r--r--   0 john       (501) staff       (20)       14 2022-04-21 15:51:17.000000 eventsourcing-9.2.8/eventsourcing.egg-info/top_level.txt
--rw-r--r--   0 john       (501) staff       (20)      781 2022-04-21 15:51:18.000000 eventsourcing-9.2.8/setup.cfg
--rw-r--r--   0 john       (501) staff       (20)     2546 2022-04-20 16:25:25.000000 eventsourcing-9.2.8/setup.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2022-04-23 16:56:20.000000 eventsourcing-9.2.9/
+-rw-r--r--   0 john       (501) staff       (20)      137 2022-03-17 22:05:19.000000 eventsourcing-9.2.9/AUTHORS
+-rw-r--r--   0 john       (501) staff       (20)     1512 2022-03-17 22:05:19.000000 eventsourcing-9.2.9/LICENSE
+-rw-r--r--   0 john       (501) staff       (20)     9017 2022-04-23 16:56:20.000000 eventsourcing-9.2.9/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)     7471 2022-03-17 22:05:19.000000 eventsourcing-9.2.9/README.md
+drwxr-xr-x   0 john       (501) staff       (20)        0 2022-04-23 16:56:20.000000 eventsourcing-9.2.9/eventsourcing/
+-rw-r--r--   0 john       (501) staff       (20)       22 2022-04-23 16:39:58.000000 eventsourcing-9.2.9/eventsourcing/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)    36097 2022-04-20 16:25:50.000000 eventsourcing-9.2.9/eventsourcing/application.py
+-rw-r--r--   0 john       (501) staff       (20)     3093 2022-04-20 16:25:25.000000 eventsourcing-9.2.9/eventsourcing/cipher.py
+-rw-r--r--   0 john       (501) staff       (20)      385 2022-03-17 22:05:19.000000 eventsourcing-9.2.9/eventsourcing/compressor.py
+-rw-r--r--   0 john       (501) staff       (20)     1489 2022-04-20 16:25:50.000000 eventsourcing-9.2.9/eventsourcing/dispatch.py
+-rw-r--r--   0 john       (501) staff       (20)    52381 2022-04-23 15:35:21.000000 eventsourcing-9.2.9/eventsourcing/domain.py
+-rw-r--r--   0 john       (501) staff       (20)     4653 2022-03-17 22:05:19.000000 eventsourcing-9.2.9/eventsourcing/interface.py
+-rw-r--r--   0 john       (501) staff       (20)    37426 2022-04-20 16:25:50.000000 eventsourcing-9.2.9/eventsourcing/persistence.py
+-rw-r--r--   0 john       (501) staff       (20)     6485 2022-03-17 22:05:19.000000 eventsourcing-9.2.9/eventsourcing/popo.py
+-rw-r--r--   0 john       (501) staff       (20)    36635 2022-04-20 16:25:25.000000 eventsourcing-9.2.9/eventsourcing/postgres.py
+-rw-r--r--   0 john       (501) staff       (20)        0 2022-03-15 14:47:08.000000 eventsourcing-9.2.9/eventsourcing/py.typed
+-rw-r--r--   0 john       (501) staff       (20)    18860 2022-04-20 16:25:25.000000 eventsourcing-9.2.9/eventsourcing/sqlite.py
+-rw-r--r--   0 john       (501) staff       (20)    45604 2022-04-22 12:11:48.000000 eventsourcing-9.2.9/eventsourcing/system.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2022-04-23 16:56:20.000000 eventsourcing-9.2.9/eventsourcing/tests/
+-rw-r--r--   0 john       (501) staff       (20)        0 2021-11-19 02:39:53.000000 eventsourcing-9.2.9/eventsourcing/tests/__init__.py
+-rw-r--r--   0 john       (501) staff       (20)    17022 2022-04-20 16:25:25.000000 eventsourcing-9.2.9/eventsourcing/tests/application.py
+-rw-r--r--   0 john       (501) staff       (20)     3256 2022-04-20 16:25:25.000000 eventsourcing-9.2.9/eventsourcing/tests/domain.py
+-rw-r--r--   0 john       (501) staff       (20)    43485 2022-04-20 16:25:25.000000 eventsourcing-9.2.9/eventsourcing/tests/persistence.py
+-rw-r--r--   0 john       (501) staff       (20)     1340 2022-03-17 22:05:20.000000 eventsourcing-9.2.9/eventsourcing/tests/postgres_utils.py
+-rw-r--r--   0 john       (501) staff       (20)     8451 2022-04-20 16:25:50.000000 eventsourcing-9.2.9/eventsourcing/utils.py
+drwxr-xr-x   0 john       (501) staff       (20)        0 2022-04-23 16:56:20.000000 eventsourcing-9.2.9/eventsourcing.egg-info/
+-rw-r--r--   0 john       (501) staff       (20)     9017 2022-04-23 16:56:20.000000 eventsourcing-9.2.9/eventsourcing.egg-info/PKG-INFO
+-rw-r--r--   0 john       (501) staff       (20)      789 2022-04-23 16:56:20.000000 eventsourcing-9.2.9/eventsourcing.egg-info/SOURCES.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2022-04-23 16:56:20.000000 eventsourcing-9.2.9/eventsourcing.egg-info/dependency_links.txt
+-rw-r--r--   0 john       (501) staff       (20)        1 2021-12-15 16:43:28.000000 eventsourcing-9.2.9/eventsourcing.egg-info/not-zip-safe
+-rw-r--r--   0 john       (501) staff       (20)      480 2022-04-23 16:56:20.000000 eventsourcing-9.2.9/eventsourcing.egg-info/requires.txt
+-rw-r--r--   0 john       (501) staff       (20)       14 2022-04-23 16:56:20.000000 eventsourcing-9.2.9/eventsourcing.egg-info/top_level.txt
+-rw-r--r--   0 john       (501) staff       (20)      781 2022-04-23 16:56:20.000000 eventsourcing-9.2.9/setup.cfg
+-rw-r--r--   0 john       (501) staff       (20)     2546 2022-04-20 16:25:25.000000 eventsourcing-9.2.9/setup.py
```

### Comparing `eventsourcing-9.2.8/LICENSE` & `eventsourcing-9.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/PKG-INFO` & `eventsourcing-9.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventsourcing
-Version: 9.2.8
+Version: 9.2.9
 Summary: Event sourcing in Python
 Home-page: https://github.com/pyeventsourcing/eventsourcing
 Author: John Bywater
 Author-email: john.bywater@appropriatesoftware.net
 License: BSD-3-Clause
 Description: A library for event sourcing in Python.
```

### Comparing `eventsourcing-9.2.8/README.md` & `eventsourcing-9.2.9/README.md`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/application.py` & `eventsourcing-9.2.9/eventsourcing/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/cipher.py` & `eventsourcing-9.2.9/eventsourcing/cipher.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/dispatch.py` & `eventsourcing-9.2.9/eventsourcing/dispatch.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/domain.py` & `eventsourcing-9.2.9/eventsourcing/domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -570,16 +570,19 @@
 
     def __init__(self, event_decorator: CommandMethodDecorator):
         """
 
         :param CommandMethodDecorator event_decorator:
         """
         self.event_decorator = event_decorator
-        self.__qualname__ = event_decorator.decorated_method.__qualname__
+        self.__module__ = event_decorator.decorated_method.__module__
         self.__name__ = event_decorator.decorated_method.__name__
+        self.__qualname__ = event_decorator.decorated_method.__qualname__
+        self.__annotations__ = event_decorator.decorated_method.__annotations__
+        self.__doc__ = event_decorator.decorated_method.__doc__
 
 
 class BoundCommandMethodDecorator:
     """
     Wraps an EventDecorator instance when attribute is accessed
     on an aggregate so that the aggregate methods can be accessed.
     """
@@ -587,16 +590,19 @@
     def __init__(self, event_decorator: CommandMethodDecorator, aggregate: Aggregate):
         """
 
         :param CommandMethodDecorator event_decorator:
         :param Aggregate aggregate:
         """
         self.event_decorator = event_decorator
-        self.__qualname__ = event_decorator.decorated_method.__qualname__
+        self.__module__ = event_decorator.decorated_method.__module__
         self.__name__ = event_decorator.decorated_method.__name__
+        self.__qualname__ = event_decorator.decorated_method.__qualname__
+        self.__annotations__ = event_decorator.decorated_method.__annotations__
+        self.__doc__ = event_decorator.decorated_method.__doc__
         self.aggregate = aggregate
 
     def trigger(self, *args: Any, **kwargs: Any) -> None:
         kwargs = _coerce_args_to_kwargs(
             self.event_decorator.decorated_method, args, kwargs
         )
         event_cls = decorated_event_classes[self.event_decorator]
```

### Comparing `eventsourcing-9.2.8/eventsourcing/interface.py` & `eventsourcing-9.2.9/eventsourcing/interface.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/persistence.py` & `eventsourcing-9.2.9/eventsourcing/persistence.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/popo.py` & `eventsourcing-9.2.9/eventsourcing/popo.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/postgres.py` & `eventsourcing-9.2.9/eventsourcing/postgres.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/sqlite.py` & `eventsourcing-9.2.9/eventsourcing/sqlite.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/system.py` & `eventsourcing-9.2.9/eventsourcing/system.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/tests/application.py` & `eventsourcing-9.2.9/eventsourcing/tests/application.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/tests/domain.py` & `eventsourcing-9.2.9/eventsourcing/tests/domain.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/tests/persistence.py` & `eventsourcing-9.2.9/eventsourcing/tests/persistence.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/tests/postgres_utils.py` & `eventsourcing-9.2.9/eventsourcing/tests/postgres_utils.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing/utils.py` & `eventsourcing-9.2.9/eventsourcing/utils.py`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/eventsourcing.egg-info/PKG-INFO` & `eventsourcing-9.2.9/eventsourcing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventsourcing
-Version: 9.2.8
+Version: 9.2.9
 Summary: Event sourcing in Python
 Home-page: https://github.com/pyeventsourcing/eventsourcing
 Author: John Bywater
 Author-email: john.bywater@appropriatesoftware.net
 License: BSD-3-Clause
 Description: A library for event sourcing in Python.
```

### Comparing `eventsourcing-9.2.8/eventsourcing.egg-info/SOURCES.txt` & `eventsourcing-9.2.9/eventsourcing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/setup.cfg` & `eventsourcing-9.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `eventsourcing-9.2.8/setup.py` & `eventsourcing-9.2.9/setup.py`

 * *Files identical despite different names*


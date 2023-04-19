# Comparing `tmp/shep-0.3.0.tar.gz` & `tmp/shep-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shep-0.3.0.tar", last modified: Mon Nov  7 09:09:17 2022, max compression
+gzip compressed data, was "shep-0.3.1.tar", last modified: Wed Apr 19 10:39:49 2023, max compression
```

## Comparing `shep-0.3.0.tar` & `shep-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,33 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-07 09:09:17.156317 shep-0.3.0/
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-01-31 08:24:17.000000 shep-0.3.0/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      649 2022-11-07 09:09:17.156317 shep-0.3.0/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      664 2022-11-07 09:09:17.156317 shep-0.3.0/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      154 2022-10-13 07:26:39.000000 shep-0.3.0/setup.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-07 09:09:17.152983 shep-0.3.0/shep/
--rw-r--r--   0 lash      (1000) lash      (1000)       25 2022-01-31 08:23:47.000000 shep-0.3.0/shep/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      837 2022-10-13 07:26:39.000000 shep-0.3.0/shep/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)     7469 2022-11-07 00:20:20.000000 shep-0.3.0/shep/persist.py
--rw-r--r--   0 lash      (1000) lash      (1000)    22052 2022-11-07 08:57:46.000000 shep-0.3.0/shep/state.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-07 09:09:17.156317 shep-0.3.0/shep/store/
--rw-r--r--   0 lash      (1000) lash      (1000)      255 2022-10-13 07:26:39.000000 shep-0.3.0/shep/store/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5998 2022-11-06 23:27:23.000000 shep-0.3.0/shep/store/file.py
--rw-r--r--   0 lash      (1000) lash      (1000)      544 2022-10-13 07:26:39.000000 shep-0.3.0/shep/store/noop.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2427 2022-10-13 07:26:39.000000 shep-0.3.0/shep/store/redis.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3110 2022-10-13 07:26:39.000000 shep-0.3.0/shep/store/rocksdb.py
--rw-r--r--   0 lash      (1000) lash      (1000)       59 2022-04-09 16:10:56.000000 shep-0.3.0/shep/verify.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2022-11-07 09:09:17.156317 shep-0.3.0/shep.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      649 2022-11-07 09:09:17.000000 shep-0.3.0/shep.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      340 2022-11-07 09:09:17.000000 shep-0.3.0/shep.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2022-11-07 09:09:17.000000 shep-0.3.0/shep.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       53 2022-11-07 09:09:17.000000 shep-0.3.0/shep.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        5 2022-11-07 09:09:17.000000 shep-0.3.0/shep.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:39:49.573293 shep-0.3.1/
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-01-31 08:24:17.000000 shep-0.3.1/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 10:39:49.573293 shep-0.3.1/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      664 2023-04-19 10:39:49.576626 shep-0.3.1/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      154 2022-10-13 07:26:39.000000 shep-0.3.1/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:39:49.573293 shep-0.3.1/shep/
+-rw-r--r--   0 lash      (1000) lash      (1000)       25 2022-01-31 08:23:47.000000 shep-0.3.1/shep/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      837 2022-10-13 07:26:39.000000 shep-0.3.1/shep/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7888 2023-04-19 10:37:38.000000 shep-0.3.1/shep/persist.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    22478 2023-04-19 10:37:04.000000 shep-0.3.1/shep/state.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:39:49.573293 shep-0.3.1/shep/store/
+-rw-r--r--   0 lash      (1000) lash      (1000)      255 2022-10-13 07:26:39.000000 shep-0.3.1/shep/store/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5998 2022-11-11 05:57:07.000000 shep-0.3.1/shep/store/file.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      544 2022-10-13 07:26:39.000000 shep-0.3.1/shep/store/noop.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2427 2022-10-13 07:26:39.000000 shep-0.3.1/shep/store/redis.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3110 2022-10-13 07:26:39.000000 shep-0.3.1/shep/store/rocksdb.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       59 2022-04-09 16:10:56.000000 shep-0.3.1/shep/verify.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:39:49.573293 shep-0.3.1/shep.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 10:39:49.000000 shep-0.3.1/shep.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      521 2023-04-19 10:39:49.000000 shep-0.3.1/shep.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-19 10:39:49.000000 shep-0.3.1/shep.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       53 2023-04-19 10:39:49.000000 shep-0.3.1/shep.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        5 2023-04-19 10:39:49.000000 shep-0.3.1/shep.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:39:49.573293 shep-0.3.1/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     9060 2022-11-11 05:57:07.000000 shep-0.3.1/tests/test_file.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3307 2022-02-04 22:14:27.000000 shep-0.3.1/tests/test_item.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2035 2022-10-13 07:26:39.000000 shep-0.3.1/tests/test_noop.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3171 2022-10-13 07:26:39.000000 shep-0.3.1/tests/test_redis.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1438 2022-01-31 10:05:15.000000 shep-0.3.1/tests/test_report.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2626 2022-10-13 07:26:39.000000 shep-0.3.1/tests/test_rocksdb.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     9711 2023-04-19 10:31:02.000000 shep-0.3.1/tests/test_state.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2208 2022-11-11 05:57:07.000000 shep-0.3.1/tests/test_store.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      666 2022-11-11 05:57:07.000000 shep-0.3.1/tests/test_verify.py
```

### Comparing `shep-0.3.0/LICENSE` & `shep-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shep-0.3.0/PKG-INFO` & `shep-0.3.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shep
-Version: 0.3.0
+Version: 0.3.1
 Summary: Multi-state key stores using bit masks
 Home-page: https://git.defalsify.org/python-shep
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPL3
 Keywords: dict,queue
 Classifier: Programming Language :: Python :: 3
```

### Comparing `shep-0.3.0/setup.cfg` & `shep-0.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shep
-version = 0.3.0
+version = 0.3.1
 description = Multi-state key stores using bit masks
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/python-shep
 keywords = 
 	dict
 	queue
```

### Comparing `shep-0.3.0/shep/error.py` & `shep-0.3.1/shep/error.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.0/shep/persist.py` & `shep-0.3.1/shep/persist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # standard imports
 import datetime
 
 # local imports
 from .state import (
         State,
+        split_elements,
         )
 from .error import (
         StateItemExists,
         StateLockedKey,
+        StateExists,
         )
 
 
 class PersistedState(State):
     """Adapter for persisting state changes and synchronising states between memory and persisted backend.
 
     :param factory: A function capable of returning a persisted store from a single path argument.
@@ -126,25 +128,40 @@
         See shep.state.State.move
         """
         from_state = self.state(key)
         to_state = super(PersistedState, self).move(key, to_state)
         return self.__movestore(key, from_state, to_state)
 
 
+    def __ensure_parts(self, state):
+        if self.is_pure(state):
+            return
+        state_name = self.name(state)
+        parts = split_elements(state_name)
+        for k in parts:
+            try:
+                self.add(k)
+            except StateExists:
+                pass
+            self.__ensure_store(k)
+
+
     # common procedure for safely moving a persisted resource from one state to another.
     def __movestore(self, key, from_state, to_state):
         k_from = self.name(from_state)
         k_to = self.name(to_state)
 
         self.__ensure_store(k_to)
 
         contents = self.__stores[k_from].get(key)
         self.__stores[k_to].put(key, contents)
         self.__stores[k_from].remove(key)
 
+        self.__ensure_parts(to_state)
+
         self.register_modify(key)
 
         self.sync(to_state)
 
         return to_state
 
 
@@ -241,13 +258,13 @@
         state = self.state(key)
         k = self.name(state)
         return self.__stores[k].modified(key)
 
 
     def add(self, key):
         self.__ensure_store(key)
-        super(PersistedState, self).add(key)
+        return super(PersistedState, self).add(key)
 
 
     def alias(self, key, *args):
         self.__ensure_store(key)
         super(PersistedState, self).alias(key, *args)
```

### Comparing `shep-0.3.0/shep/state.py` & `shep-0.3.1/shep/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,14 +201,15 @@
         :type k: str
         :raises shep.error.StateExists: State name is already registered
         """
         v = 1 << self.__c
         k = self.__check_name(k)
         v = self.__check_value(v)
         self.__set(k, v)
+        return v
 
 
     def to_name(self, k):
         if k == None:
             k = 0
         return self.name(k)
 
@@ -301,20 +302,33 @@
 
         if len(r) == 1:
             return self.name(v)
 
         return join_elements(r) #'_' + '.'.join(r)
 
 
-    def from_elements(self, k):
+    def from_elements(self, k, create_missing=False):
         r = 0
         if k[0] != '_':
             raise ValueError('elements string must start with underscore (_), got {}'.format(k))
         for v in k[1:].split('__'):
-            r |= self.from_name(v) 
+            state = None
+            print("state {} {}".format(v, k))
+            try:
+                state = self.from_name(v) 
+            except AttributeError as e:
+                pass
+
+            if state == None:
+                if not create_missing: 
+                    raise StateInvalid(v)
+                state = self.add(v)
+            print("state {} {} {}".format(v, k, state))
+
+            r |= state
         return r
 
 
     def name(self, v):
         """Retrieve that string representation of the state attribute represented by the given state integer value.
         
         :param v: State integer
```

### Comparing `shep-0.3.0/shep/store/file.py` & `shep-0.3.1/shep/store/file.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.0/shep/store/noop.py` & `shep-0.3.1/shep/store/noop.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.0/shep/store/redis.py` & `shep-0.3.1/shep/store/redis.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.0/shep/store/rocksdb.py` & `shep-0.3.1/shep/store/rocksdb.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.0/shep.egg-info/PKG-INFO` & `shep-0.3.1/shep.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shep
-Version: 0.3.0
+Version: 0.3.1
 Summary: Multi-state key stores using bit masks
 Home-page: https://git.defalsify.org/python-shep
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPL3
 Keywords: dict,queue
 Classifier: Programming Language :: Python :: 3
```


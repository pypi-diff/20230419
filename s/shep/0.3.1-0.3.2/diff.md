# Comparing `tmp/shep-0.3.1.tar.gz` & `tmp/shep-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shep-0.3.1.tar", last modified: Wed Apr 19 10:39:49 2023, max compression
+gzip compressed data, was "shep-0.3.2.tar", last modified: Wed Apr 19 10:42:49 2023, max compression
```

## Comparing `shep-0.3.1.tar` & `shep-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:39:49.573293 shep-0.3.1/
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-01-31 08:24:17.000000 shep-0.3.1/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 10:39:49.573293 shep-0.3.1/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      664 2023-04-19 10:39:49.576626 shep-0.3.1/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      154 2022-10-13 07:26:39.000000 shep-0.3.1/setup.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:39:49.573293 shep-0.3.1/shep/
--rw-r--r--   0 lash      (1000) lash      (1000)       25 2022-01-31 08:23:47.000000 shep-0.3.1/shep/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      837 2022-10-13 07:26:39.000000 shep-0.3.1/shep/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)     7888 2023-04-19 10:37:38.000000 shep-0.3.1/shep/persist.py
--rw-r--r--   0 lash      (1000) lash      (1000)    22478 2023-04-19 10:37:04.000000 shep-0.3.1/shep/state.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:39:49.573293 shep-0.3.1/shep/store/
--rw-r--r--   0 lash      (1000) lash      (1000)      255 2022-10-13 07:26:39.000000 shep-0.3.1/shep/store/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5998 2022-11-11 05:57:07.000000 shep-0.3.1/shep/store/file.py
--rw-r--r--   0 lash      (1000) lash      (1000)      544 2022-10-13 07:26:39.000000 shep-0.3.1/shep/store/noop.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2427 2022-10-13 07:26:39.000000 shep-0.3.1/shep/store/redis.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3110 2022-10-13 07:26:39.000000 shep-0.3.1/shep/store/rocksdb.py
--rw-r--r--   0 lash      (1000) lash      (1000)       59 2022-04-09 16:10:56.000000 shep-0.3.1/shep/verify.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:39:49.573293 shep-0.3.1/shep.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 10:39:49.000000 shep-0.3.1/shep.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      521 2023-04-19 10:39:49.000000 shep-0.3.1/shep.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-19 10:39:49.000000 shep-0.3.1/shep.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       53 2023-04-19 10:39:49.000000 shep-0.3.1/shep.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        5 2023-04-19 10:39:49.000000 shep-0.3.1/shep.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:39:49.573293 shep-0.3.1/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     9060 2022-11-11 05:57:07.000000 shep-0.3.1/tests/test_file.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3307 2022-02-04 22:14:27.000000 shep-0.3.1/tests/test_item.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2035 2022-10-13 07:26:39.000000 shep-0.3.1/tests/test_noop.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3171 2022-10-13 07:26:39.000000 shep-0.3.1/tests/test_redis.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1438 2022-01-31 10:05:15.000000 shep-0.3.1/tests/test_report.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2626 2022-10-13 07:26:39.000000 shep-0.3.1/tests/test_rocksdb.py
--rw-r--r--   0 lash      (1000) lash      (1000)     9711 2023-04-19 10:31:02.000000 shep-0.3.1/tests/test_state.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2208 2022-11-11 05:57:07.000000 shep-0.3.1/tests/test_store.py
--rw-r--r--   0 lash      (1000) lash      (1000)      666 2022-11-11 05:57:07.000000 shep-0.3.1/tests/test_verify.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:42:49.133292 shep-0.3.2/
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-01-31 08:24:17.000000 shep-0.3.2/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 10:42:49.136625 shep-0.3.2/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      664 2023-04-19 10:42:49.136625 shep-0.3.2/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      154 2022-10-13 07:26:39.000000 shep-0.3.2/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:42:49.133292 shep-0.3.2/shep/
+-rw-r--r--   0 lash      (1000) lash      (1000)       25 2022-01-31 08:23:47.000000 shep-0.3.2/shep/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      837 2022-10-13 07:26:39.000000 shep-0.3.2/shep/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7888 2023-04-19 10:37:38.000000 shep-0.3.2/shep/persist.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    22374 2023-04-19 10:41:08.000000 shep-0.3.2/shep/state.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:42:49.133292 shep-0.3.2/shep/store/
+-rw-r--r--   0 lash      (1000) lash      (1000)      255 2022-10-13 07:26:39.000000 shep-0.3.2/shep/store/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5998 2022-11-11 05:57:07.000000 shep-0.3.2/shep/store/file.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      544 2022-10-13 07:26:39.000000 shep-0.3.2/shep/store/noop.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2427 2022-10-13 07:26:39.000000 shep-0.3.2/shep/store/redis.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3110 2022-10-13 07:26:39.000000 shep-0.3.2/shep/store/rocksdb.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       59 2022-04-09 16:10:56.000000 shep-0.3.2/shep/verify.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:42:49.133292 shep-0.3.2/shep.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      649 2023-04-19 10:42:49.000000 shep-0.3.2/shep.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      521 2023-04-19 10:42:49.000000 shep-0.3.2/shep.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-19 10:42:49.000000 shep-0.3.2/shep.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       53 2023-04-19 10:42:49.000000 shep-0.3.2/shep.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        5 2023-04-19 10:42:49.000000 shep-0.3.2/shep.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-19 10:42:49.133292 shep-0.3.2/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     9060 2022-11-11 05:57:07.000000 shep-0.3.2/tests/test_file.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3307 2022-02-04 22:14:27.000000 shep-0.3.2/tests/test_item.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2035 2022-10-13 07:26:39.000000 shep-0.3.2/tests/test_noop.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3171 2022-10-13 07:26:39.000000 shep-0.3.2/tests/test_redis.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1438 2022-01-31 10:05:15.000000 shep-0.3.2/tests/test_report.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2626 2022-10-13 07:26:39.000000 shep-0.3.2/tests/test_rocksdb.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     9711 2023-04-19 10:31:02.000000 shep-0.3.2/tests/test_state.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2208 2022-11-11 05:57:07.000000 shep-0.3.2/tests/test_store.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      666 2022-11-11 05:57:07.000000 shep-0.3.2/tests/test_verify.py
```

### Comparing `shep-0.3.1/LICENSE` & `shep-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/setup.cfg` & `shep-0.3.2/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shep
-version = 0.3.1
+version = 0.3.2
 description = Multi-state key stores using bit masks
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/python-shep
 keywords = 
 	dict
 	queue
```

### Comparing `shep-0.3.1/shep/error.py` & `shep-0.3.2/shep/error.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/shep/persist.py` & `shep-0.3.2/shep/persist.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/shep/state.py` & `shep-0.3.2/shep/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -308,25 +308,23 @@
 
     def from_elements(self, k, create_missing=False):
         r = 0
         if k[0] != '_':
             raise ValueError('elements string must start with underscore (_), got {}'.format(k))
         for v in k[1:].split('__'):
             state = None
-            print("state {} {}".format(v, k))
             try:
                 state = self.from_name(v) 
             except AttributeError as e:
                 pass
 
             if state == None:
                 if not create_missing: 
                     raise StateInvalid(v)
                 state = self.add(v)
-            print("state {} {} {}".format(v, k, state))
 
             r |= state
         return r
 
 
     def name(self, v):
         """Retrieve that string representation of the state attribute represented by the given state integer value.
```

### Comparing `shep-0.3.1/shep/store/file.py` & `shep-0.3.2/shep/store/file.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/shep/store/noop.py` & `shep-0.3.2/shep/store/noop.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/shep/store/redis.py` & `shep-0.3.2/shep/store/redis.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/shep/store/rocksdb.py` & `shep-0.3.2/shep/store/rocksdb.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/shep.egg-info/SOURCES.txt` & `shep-0.3.2/shep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/tests/test_file.py` & `shep-0.3.2/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/tests/test_item.py` & `shep-0.3.2/tests/test_item.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/tests/test_noop.py` & `shep-0.3.2/tests/test_noop.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/tests/test_redis.py` & `shep-0.3.2/tests/test_redis.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/tests/test_report.py` & `shep-0.3.2/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/tests/test_rocksdb.py` & `shep-0.3.2/tests/test_rocksdb.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/tests/test_state.py` & `shep-0.3.2/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/tests/test_store.py` & `shep-0.3.2/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `shep-0.3.1/tests/test_verify.py` & `shep-0.3.2/tests/test_verify.py`

 * *Files identical despite different names*


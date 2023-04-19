# Comparing `tmp/dkredis-0.1.8.tar.gz` & `tmp/dkredis-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkredis-0.1.8.tar", last modified: Wed Apr 19 11:54:55 2023, max compression
+gzip compressed data, was "dkredis-0.1.9.tar", last modified: Wed Apr 19 12:04:44 2023, max compression
```

## Comparing `dkredis-0.1.8.tar` & `dkredis-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:54:55.875089 dkredis-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-19 11:54:55.875089 dkredis-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-19 11:54:44.000000 dkredis-0.1.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:54:55.875089 dkredis-0.1.8/dkredis/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 11:54:44.000000 dkredis-0.1.8/dkredis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-04-19 11:54:44.000000 dkredis-0.1.8/dkredis/dkredis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-04-19 11:54:44.000000 dkredis-0.1.8/dkredis/rediscache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 11:54:55.875089 dkredis-0.1.8/dkredis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-19 11:54:55.000000 dkredis-0.1.8/dkredis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-19 11:54:55.000000 dkredis-0.1.8/dkredis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:54:55.000000 dkredis-0.1.8/dkredis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 11:54:55.000000 dkredis-0.1.8/dkredis.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 11:54:55.000000 dkredis-0.1.8/dkredis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 11:54:55.000000 dkredis-0.1.8/dkredis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-19 11:54:55.875089 dkredis-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-19 11:54:44.000000 dkredis-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:04:44.772900 dkredis-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-19 12:04:31.000000 dkredis-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-19 12:04:44.772900 dkredis-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-19 12:04:31.000000 dkredis-0.1.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:04:44.772900 dkredis-0.1.9/dkredis/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-19 12:04:31.000000 dkredis-0.1.9/dkredis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11456 2023-04-19 12:04:31.000000 dkredis-0.1.9/dkredis/dkredis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-04-19 12:04:31.000000 dkredis-0.1.9/dkredis/rediscache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 12:04:44.772900 dkredis-0.1.9/dkredis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-19 12:04:44.000000 dkredis-0.1.9/dkredis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-19 12:04:44.000000 dkredis-0.1.9/dkredis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:04:44.000000 dkredis-0.1.9/dkredis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 12:04:44.000000 dkredis-0.1.9/dkredis.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-19 12:04:44.000000 dkredis-0.1.9/dkredis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 12:04:44.000000 dkredis-0.1.9/dkredis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-19 12:04:44.772900 dkredis-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-19 12:04:31.000000 dkredis-0.1.9/setup.py
```

### Comparing `dkredis-0.1.8/PKG-INFO` & `dkredis-0.1.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: dkredis
-Version: 0.1.8
+Version: 0.1.9
 Summary: dkredis - Python interface to Redis
-Home-page: UNKNOWN
-License: UNKNOWN
+Home-page: https://github.com/datakortet/dkredis
+Author: bjorn
+Author-email: bp@datakortet.no
+License: MIT
+Keywords: redis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
 
 
 
 dkredis - Python interface to Redis
 ===================================
 
 .. image:: https://coveralls.io/repos/github/datakortet/dkredis/badge.svg?branch=master
```

### Comparing `dkredis-0.1.8/README.rst` & `dkredis-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `dkredis-0.1.8/dkredis/dkredis.py` & `dkredis-0.1.9/dkredis/dkredis.py`

 * *Files identical despite different names*

### Comparing `dkredis-0.1.8/dkredis/rediscache.py` & `dkredis-0.1.9/dkredis/rediscache.py`

 * *Files identical despite different names*

### Comparing `dkredis-0.1.8/dkredis.egg-info/PKG-INFO` & `dkredis-0.1.9/dkredis.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 Metadata-Version: 2.1
 Name: dkredis
-Version: 0.1.8
+Version: 0.1.9
 Summary: dkredis - Python interface to Redis
-Home-page: UNKNOWN
-License: UNKNOWN
+Home-page: https://github.com/datakortet/dkredis
+Author: bjorn
+Author-email: bp@datakortet.no
+License: MIT
+Keywords: redis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
+License-File: LICENSE
 
 
 
 dkredis - Python interface to Redis
 ===================================
 
 .. image:: https://coveralls.io/repos/github/datakortet/dkredis/badge.svg?branch=master
```


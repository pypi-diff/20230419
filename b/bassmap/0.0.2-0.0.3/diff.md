# Comparing `tmp/bassmap-0.0.2.tar.gz` & `tmp/bassmap-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bassmap-0.0.2.tar", last modified: Fri Apr 14 20:01:32 2023, max compression
+gzip compressed data, was "bassmap-0.0.3.tar", last modified: Wed Apr 19 00:14:51 2023, max compression
```

## Comparing `bassmap-0.0.2.tar` & `bassmap-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:01:32.695640 bassmap-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-14 20:01:19.000000 bassmap-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-14 20:01:19.000000 bassmap-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-14 20:01:32.695640 bassmap-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-14 20:01:19.000000 bassmap-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:01:32.695640 bassmap-0.0.2/bassmap/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-14 20:01:19.000000 bassmap-0.0.2/bassmap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-14 20:01:19.000000 bassmap-0.0.2/bassmap/bassmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 20:01:32.695640 bassmap-0.0.2/bassmap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-14 20:01:32.000000 bassmap-0.0.2/bassmap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-14 20:01:32.000000 bassmap-0.0.2/bassmap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 20:01:32.000000 bassmap-0.0.2/bassmap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 20:01:32.000000 bassmap-0.0.2/bassmap.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-14 20:01:32.000000 bassmap-0.0.2/bassmap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 20:01:32.000000 bassmap-0.0.2/bassmap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-14 20:01:19.000000 bassmap-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-14 20:01:32.695640 bassmap-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-14 20:01:19.000000 bassmap-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:14:51.776460 bassmap-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-19 00:14:41.000000 bassmap-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-19 00:14:41.000000 bassmap-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-19 00:14:51.776460 bassmap-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-19 00:14:41.000000 bassmap-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:14:51.776460 bassmap-0.0.3/bassmap/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-19 00:14:41.000000 bassmap-0.0.3/bassmap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4133 2023-04-19 00:14:41.000000 bassmap-0.0.3/bassmap/bassmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:14:51.776460 bassmap-0.0.3/bassmap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-19 00:14:51.000000 bassmap-0.0.3/bassmap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-19 00:14:51.000000 bassmap-0.0.3/bassmap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 00:14:51.000000 bassmap-0.0.3/bassmap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:14:51.000000 bassmap-0.0.3/bassmap.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-19 00:14:51.000000 bassmap-0.0.3/bassmap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-19 00:14:51.000000 bassmap-0.0.3/bassmap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-19 00:14:41.000000 bassmap-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-19 00:14:51.776460 bassmap-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-04-19 00:14:41.000000 bassmap-0.0.3/setup.py
```

### Comparing `bassmap-0.0.2/LICENSE` & `bassmap-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bassmap-0.0.2/PKG-INFO` & `bassmap-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bassmap
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/bassneel/bassmap
 Author: Bass Neel
 Author-email: maps.bassneel@gmail.com
 License: MIT license
 Keywords: bassmap
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bassmap-0.0.2/README.md` & `bassmap-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bassmap-0.0.2/bassmap.egg-info/PKG-INFO` & `bassmap-0.0.3/bassmap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bassmap
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python Boilerplate contains all the boilerplate you need to create a Python package.
 Home-page: https://github.com/bassneel/bassmap
 Author: Bass Neel
 Author-email: maps.bassneel@gmail.com
 License: MIT license
 Keywords: bassmap
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `bassmap-0.0.2/setup.py` & `bassmap-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='bassmap',
     name='bassmap',
     packages=find_packages(include=['bassmap', 'bassmap.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/bassneel/bassmap',
-    version='0.0.2',
+    version='0.0.3',
     zip_safe=False,
 )
```


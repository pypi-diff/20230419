# Comparing `tmp/sse-starlette-1.3.3.tar.gz` & `tmp/sse-starlette-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sse-starlette-1.3.3.tar", last modified: Sat Mar 11 18:15:28 2023, max compression
+gzip compressed data, was "sse-starlette-1.3.4.tar", last modified: Wed Apr 19 04:06:33 2023, max compression
```

## Comparing `sse-starlette-1.3.3.tar` & `sse-starlette-1.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-03-11 18:15:28.167666 sse-starlette-1.3.3/
--rw-r--r--   0 Q187392    (501) staff       (20)      395 2022-12-16 17:29:08.000000 sse-starlette-1.3.3/AUTHORS
--rw-r--r--   0 Q187392    (501) staff       (20)     1892 2023-03-11 18:12:47.000000 sse-starlette-1.3.3/CHANGELOG.md
--rw-r--r--   0 Q187392    (501) staff       (20)     1511 2022-12-16 17:29:08.000000 sse-starlette-1.3.3/LICENSE
--rw-r--r--   0 Q187392    (501) staff       (20)      103 2022-12-16 17:29:08.000000 sse-starlette-1.3.3/MANIFEST.in
--rw-r--r--   0 Q187392    (501) staff       (20)     5236 2023-03-11 18:15:28.167790 sse-starlette-1.3.3/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)     3093 2023-03-11 18:06:25.000000 sse-starlette-1.3.3/README.md
--rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-16 17:29:08.000000 sse-starlette-1.3.3/pyproject.toml
--rw-r--r--   0 Q187392    (501) staff       (20)     1800 2023-03-11 18:15:28.200551 sse-starlette-1.3.3/setup.cfg
--rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-16 17:29:08.000000 sse-starlette-1.3.3/setup.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-03-11 18:15:28.163598 sse-starlette-1.3.3/sse_starlette/
--rw-r--r--   0 Q187392    (501) staff       (20)      143 2023-03-11 18:14:34.000000 sse-starlette-1.3.3/sse_starlette/__init__.py
--rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-16 17:29:08.000000 sse-starlette-1.3.3/sse_starlette/py.typed
--rw-r--r--   0 Q187392    (501) staff       (20)    10462 2023-03-11 17:23:01.000000 sse-starlette-1.3.3/sse_starlette/sse.py
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-03-11 18:15:28.166437 sse-starlette-1.3.3/sse_starlette.egg-info/
--rw-r--r--   0 Q187392    (501) staff       (20)     5236 2023-03-11 18:15:27.000000 sse-starlette-1.3.3/sse_starlette.egg-info/PKG-INFO
--rw-r--r--   0 Q187392    (501) staff       (20)      392 2023-03-11 18:15:28.000000 sse-starlette-1.3.3/sse_starlette.egg-info/SOURCES.txt
--rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-03-11 18:15:27.000000 sse-starlette-1.3.3/sse_starlette.egg-info/dependency_links.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-03-11 18:15:27.000000 sse-starlette-1.3.3/sse_starlette.egg-info/requires.txt
--rw-r--r--   0 Q187392    (501) staff       (20)       14 2023-03-11 18:15:27.000000 sse-starlette-1.3.3/sse_starlette.egg-info/top_level.txt
-drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-03-11 18:15:28.167349 sse-starlette-1.3.3/tests/
--rw-r--r--   0 Q187392    (501) staff       (20)     3675 2022-12-16 17:29:08.000000 sse-starlette-1.3.3/tests/test_event_source_response.py
--rw-r--r--   0 Q187392    (501) staff       (20)     2811 2022-12-16 17:29:08.000000 sse-starlette-1.3.3/tests/test_sse.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-19 04:06:33.118712 sse-starlette-1.3.4/
+-rw-r--r--   0 Q187392    (501) staff       (20)      395 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/AUTHORS
+-rw-r--r--   0 Q187392    (501) staff       (20)     1892 2023-03-11 18:12:47.000000 sse-starlette-1.3.4/CHANGELOG.md
+-rw-r--r--   0 Q187392    (501) staff       (20)     1511 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/LICENSE
+-rw-r--r--   0 Q187392    (501) staff       (20)      103 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/MANIFEST.in
+-rw-r--r--   0 Q187392    (501) staff       (20)     5236 2023-04-19 04:06:33.118896 sse-starlette-1.3.4/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)     3093 2023-03-11 18:06:25.000000 sse-starlette-1.3.4/README.md
+-rw-r--r--   0 Q187392    (501) staff       (20)      106 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/pyproject.toml
+-rw-r--r--   0 Q187392    (501) staff       (20)     1800 2023-04-19 04:06:33.119660 sse-starlette-1.3.4/setup.cfg
+-rw-r--r--   0 Q187392    (501) staff       (20)      152 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/setup.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-19 04:06:33.114844 sse-starlette-1.3.4/sse_starlette/
+-rw-r--r--   0 Q187392    (501) staff       (20)      143 2023-04-19 04:05:55.000000 sse-starlette-1.3.4/sse_starlette/__init__.py
+-rw-r--r--   0 Q187392    (501) staff       (20)        0 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/sse_starlette/py.typed
+-rw-r--r--   0 Q187392    (501) staff       (20)    10462 2023-03-11 17:23:01.000000 sse-starlette-1.3.4/sse_starlette/sse.py
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-19 04:06:33.117523 sse-starlette-1.3.4/sse_starlette.egg-info/
+-rw-r--r--   0 Q187392    (501) staff       (20)     5236 2023-04-19 04:06:32.000000 sse-starlette-1.3.4/sse_starlette.egg-info/PKG-INFO
+-rw-r--r--   0 Q187392    (501) staff       (20)      392 2023-04-19 04:06:33.000000 sse-starlette-1.3.4/sse_starlette.egg-info/SOURCES.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)        1 2023-04-19 04:06:32.000000 sse-starlette-1.3.4/sse_starlette.egg-info/dependency_links.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       10 2023-04-19 04:06:32.000000 sse-starlette-1.3.4/sse_starlette.egg-info/requires.txt
+-rw-r--r--   0 Q187392    (501) staff       (20)       14 2023-04-19 04:06:32.000000 sse-starlette-1.3.4/sse_starlette.egg-info/top_level.txt
+drwxr-xr-x   0 Q187392    (501) staff       (20)        0 2023-04-19 04:06:33.118417 sse-starlette-1.3.4/tests/
+-rw-r--r--   0 Q187392    (501) staff       (20)     3675 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/tests/test_event_source_response.py
+-rw-r--r--   0 Q187392    (501) staff       (20)     2811 2022-12-16 17:29:08.000000 sse-starlette-1.3.4/tests/test_sse.py
```

### Comparing `sse-starlette-1.3.3/CHANGELOG.md` & `sse-starlette-1.3.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `sse-starlette-1.3.3/LICENSE` & `sse-starlette-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sse-starlette-1.3.3/PKG-INFO` & `sse-starlette-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sse-starlette
-Version: 1.3.3
+Version: 1.3.4
 Summary: "SSE plugin for Starlette"
 Home-page: https://github.com/sysid/sse-starlette
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `sse-starlette-1.3.3/README.md` & `sse-starlette-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `sse-starlette-1.3.3/setup.cfg` & `sse-starlette-1.3.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sse-starlette
-version = 1.3.3
+version = 1.3.4
 description = "SSE plugin for Starlette"
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 author = sysid
 author_email = sysid@gmx.de
 url = https://github.com/sysid/sse-starlette
 classifiers =
```

### Comparing `sse-starlette-1.3.3/sse_starlette/sse.py` & `sse-starlette-1.3.4/sse_starlette/sse.py`

 * *Files identical despite different names*

### Comparing `sse-starlette-1.3.3/sse_starlette.egg-info/PKG-INFO` & `sse-starlette-1.3.4/sse_starlette.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sse-starlette
-Version: 1.3.3
+Version: 1.3.4
 Summary: "SSE plugin for Starlette"
 Home-page: https://github.com/sysid/sse-starlette
 Author: sysid
 Author-email: sysid@gmx.de
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `sse-starlette-1.3.3/tests/test_event_source_response.py` & `sse-starlette-1.3.4/tests/test_event_source_response.py`

 * *Files identical despite different names*

### Comparing `sse-starlette-1.3.3/tests/test_sse.py` & `sse-starlette-1.3.4/tests/test_sse.py`

 * *Files identical despite different names*


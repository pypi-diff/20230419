# Comparing `tmp/multiPrime-2.4.2.tar.gz` & `tmp/multiPrime-2.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multiPrime-2.4.2.tar", last modified: Wed Apr 19 08:16:30 2023, max compression
+gzip compressed data, was "multiPrime-2.4.3.tar", last modified: Wed Apr 19 08:18:42 2023, max compression
```

## Comparing `multiPrime-2.4.2.tar` & `multiPrime-2.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-19 08:16:30.386035 multiPrime-2.4.2/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-04-19 08:13:53.000000 multiPrime-2.4.2/LICENSE
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16020 2023-04-19 08:16:30.385035 multiPrime-2.4.2/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    15867 2023-04-19 08:14:19.000000 multiPrime-2.4.2/README.md
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-19 08:16:30.385035 multiPrime-2.4.2/multiPrime.egg-info/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16020 2023-04-19 08:16:30.000000 multiPrime-2.4.2/multiPrime.egg-info/PKG-INFO
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      267 2023-04-19 08:16:30.000000 multiPrime-2.4.2/multiPrime.egg-info/SOURCES.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-04-19 08:16:30.000000 multiPrime-2.4.2/multiPrime.egg-info/dependency_links.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-04-19 08:16:30.000000 multiPrime-2.4.2/multiPrime.egg-info/entry_points.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-04-19 08:16:30.000000 multiPrime-2.4.2/multiPrime.egg-info/top_level.txt
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-04-19 08:16:30.386035 multiPrime-2.4.2/setup.cfg
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1795 2023-04-19 08:13:53.000000 multiPrime-2.4.2/setup.py
-drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-19 08:16:30.385035 multiPrime-2.4.2/src/
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-04-19 08:14:29.000000 multiPrime-2.4.2/src/__init__.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-04-19 08:16:04.000000 multiPrime-2.4.2/src/_version.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-04-19 08:14:29.000000 multiPrime-2.4.2/src/main.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    85935 2023-04-19 08:14:29.000000 multiPrime-2.4.2/src/src.py
--rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    25251 2023-04-19 08:14:29.000000 multiPrime-2.4.2/src/utils.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-19 08:18:42.136580 multiPrime-2.4.3/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1126 2023-04-19 08:13:53.000000 multiPrime-2.4.3/LICENSE
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16020 2023-04-19 08:18:42.136580 multiPrime-2.4.3/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    15867 2023-04-19 08:14:19.000000 multiPrime-2.4.3/README.md
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-19 08:18:42.135580 multiPrime-2.4.3/multiPrime.egg-info/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    16020 2023-04-19 08:18:42.000000 multiPrime-2.4.3/multiPrime.egg-info/PKG-INFO
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)      267 2023-04-19 08:18:42.000000 multiPrime-2.4.3/multiPrime.egg-info/SOURCES.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)        1 2023-04-19 08:18:42.000000 multiPrime-2.4.3/multiPrime.egg-info/dependency_links.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       52 2023-04-19 08:18:42.000000 multiPrime-2.4.3/multiPrime.egg-info/entry_points.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       11 2023-04-19 08:18:42.000000 multiPrime-2.4.3/multiPrime.egg-info/top_level.txt
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       38 2023-04-19 08:18:42.136580 multiPrime-2.4.3/setup.cfg
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     1795 2023-04-19 08:13:53.000000 multiPrime-2.4.3/setup.py
+drwxr-xr-x   0 yangjunbo  (1044) microbe   (1000)        0 2023-04-19 08:18:42.136580 multiPrime-2.4.3/src/
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       35 2023-04-19 08:14:29.000000 multiPrime-2.4.3/src/__init__.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)       23 2023-04-19 08:18:27.000000 multiPrime-2.4.3/src/_version.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)     2402 2023-04-19 08:18:18.000000 multiPrime-2.4.3/src/main.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    85935 2023-04-19 08:14:29.000000 multiPrime-2.4.3/src/src.py
+-rw-r--r--   0 yangjunbo  (1044) microbe   (1000)    25251 2023-04-19 08:14:29.000000 multiPrime-2.4.3/src/utils.py
```

### Comparing `multiPrime-2.4.2/LICENSE` & `multiPrime-2.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multiPrime-2.4.2/PKG-INFO` & `multiPrime-2.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.4.2
+Version: 2.4.3
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
```

### Comparing `multiPrime-2.4.2/README.md` & `multiPrime-2.4.3/README.md`

 * *Files identical despite different names*

### Comparing `multiPrime-2.4.2/multiPrime.egg-info/PKG-INFO` & `multiPrime-2.4.3/multiPrime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multiPrime
-Version: 2.4.2
+Version: 2.4.3
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # multiPrime
```

### Comparing `multiPrime-2.4.2/setup.py` & `multiPrime-2.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.4.2/src/main.py` & `multiPrime-2.4.3/src/main.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.4.2/src/src.py` & `multiPrime-2.4.3/src/src.py`

 * *Files identical despite different names*

### Comparing `multiPrime-2.4.2/src/utils.py` & `multiPrime-2.4.3/src/utils.py`

 * *Files identical despite different names*


# Comparing `tmp/bp_data_fabric-0.0.5.tar.gz` & `tmp/bp_data_fabric-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_fabric-0.0.5.tar", last modified: Wed Apr 19 07:06:59 2023, max compression
+gzip compressed data, was "bp_data_fabric-0.0.6.tar", last modified: Wed Apr 19 07:23:18 2023, max compression
```

## Comparing `bp_data_fabric-0.0.5.tar` & `bp_data_fabric-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:06:59.626255 bp_data_fabric-0.0.5/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-0.0.5/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-19 07:06:59.625918 bp_data_fabric-0.0.5/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-0.0.5/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:06:59.624913 bp_data_fabric-0.0.5/bp_data_fabric.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-19 07:06:59.000000 bp_data_fabric-0.0.5/bp_data_fabric.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      239 2023-04-19 07:06:59.000000 bp_data_fabric-0.0.5/bp_data_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-19 07:06:59.000000 bp_data_fabric-0.0.5/bp_data_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-19 07:06:59.000000 bp_data_fabric-0.0.5/bp_data_fabric.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-04-19 07:06:59.000000 bp_data_fabric-0.0.5/bp_data_fabric.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:06:59.625371 bp_data_fabric-0.0.5/data_fabric/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1071 2023-04-18 05:57:17.000000 bp_data_fabric-0.0.5/data_fabric/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-19 07:06:59.626353 bp_data_fabric-0.0.5/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      602 2023-04-19 07:06:14.000000 bp_data_fabric-0.0.5/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:23:18.926349 bp_data_fabric-0.0.6/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-0.0.6/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-19 07:23:18.926037 bp_data_fabric-0.0.6/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-0.0.6/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:23:18.924640 bp_data_fabric-0.0.6/bp_data_fabric.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-19 07:23:18.000000 bp_data_fabric-0.0.6/bp_data_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      239 2023-04-19 07:23:18.000000 bp_data_fabric-0.0.6/bp_data_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-19 07:23:18.000000 bp_data_fabric-0.0.6/bp_data_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-19 07:23:18.000000 bp_data_fabric-0.0.6/bp_data_fabric.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-04-19 07:23:18.000000 bp_data_fabric-0.0.6/bp_data_fabric.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 07:23:18.925130 bp_data_fabric-0.0.6/data_fabric/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1071 2023-04-18 05:57:17.000000 bp_data_fabric-0.0.6/data_fabric/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-19 07:23:18.926452 bp_data_fabric-0.0.6/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      602 2023-04-19 07:22:15.000000 bp_data_fabric-0.0.6/setup.py
```

### Comparing `bp_data_fabric-0.0.5/LICENSE` & `bp_data_fabric-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-0.0.5/data_fabric/__init__.py` & `bp_data_fabric-0.0.6/data_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-0.0.5/setup.py` & `bp_data_fabric-0.0.6/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bp_data_fabric",
-    version="0.0.5",
+    version="0.0.6",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```


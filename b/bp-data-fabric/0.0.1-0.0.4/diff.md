# Comparing `tmp/bp_data_fabric-0.0.1.tar.gz` & `tmp/bp_data_fabric-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_fabric-0.0.1.tar", last modified: Wed Apr 19 05:47:39 2023, max compression
+gzip compressed data, was "bp_data_fabric-0.0.4.tar", last modified: Wed Apr 19 06:55:51 2023, max compression
```

## Comparing `bp_data_fabric-0.0.1.tar` & `bp_data_fabric-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 05:47:39.664873 bp_data_fabric-0.0.1/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-0.0.1/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-19 05:47:39.664554 bp_data_fabric-0.0.1/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-0.0.1/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 05:47:39.663177 bp_data_fabric-0.0.1/bp_data_fabric.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-19 05:47:39.000000 bp_data_fabric-0.0.1/bp_data_fabric.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      239 2023-04-19 05:47:39.000000 bp_data_fabric-0.0.1/bp_data_fabric.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-19 05:47:39.000000 bp_data_fabric-0.0.1/bp_data_fabric.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-19 05:47:39.000000 bp_data_fabric-0.0.1/bp_data_fabric.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-04-19 05:47:39.000000 bp_data_fabric-0.0.1/bp_data_fabric.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 05:47:39.663649 bp_data_fabric-0.0.1/data_fabric/
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1071 2023-04-18 05:57:17.000000 bp_data_fabric-0.0.1/data_fabric/__init__.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-19 05:47:39.664976 bp_data_fabric-0.0.1/setup.cfg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      602 2023-04-19 05:46:54.000000 bp_data_fabric-0.0.1/setup.py
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 06:55:51.299715 bp_data_fabric-0.0.4/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-13 05:40:39.000000 bp_data_fabric-0.0.4/LICENSE
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-19 06:55:51.299373 bp_data_fabric-0.0.4/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       28 2023-04-13 05:35:21.000000 bp_data_fabric-0.0.4/README.md
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 06:55:51.298559 bp_data_fabric-0.0.4/bp_data_fabric.egg-info/
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      286 2023-04-19 06:55:51.000000 bp_data_fabric-0.0.4/bp_data_fabric.egg-info/PKG-INFO
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      239 2023-04-19 06:55:51.000000 bp_data_fabric-0.0.4/bp_data_fabric.egg-info/SOURCES.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-04-19 06:55:51.000000 bp_data_fabric-0.0.4/bp_data_fabric.egg-info/dependency_links.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-04-19 06:55:51.000000 bp_data_fabric-0.0.4/bp_data_fabric.egg-info/requires.txt
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       12 2023-04-19 06:55:51.000000 bp_data_fabric-0.0.4/bp_data_fabric.egg-info/top_level.txt
+drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-04-19 06:55:51.298942 bp_data_fabric-0.0.4/data_fabric/
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1071 2023-04-18 05:57:17.000000 bp_data_fabric-0.0.4/data_fabric/__init__.py
+-rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-04-19 06:55:51.299839 bp_data_fabric-0.0.4/setup.cfg
+-rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)      602 2023-04-19 06:54:27.000000 bp_data_fabric-0.0.4/setup.py
```

### Comparing `bp_data_fabric-0.0.1/LICENSE` & `bp_data_fabric-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-0.0.1/data_fabric/__init__.py` & `bp_data_fabric-0.0.4/data_fabric/__init__.py`

 * *Files identical despite different names*

### Comparing `bp_data_fabric-0.0.1/setup.py` & `bp_data_fabric-0.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="bp_data_fabric",
-    version="0.0.1",
+    version="0.0.4",
     author="Bluepinapple",
     author_email="viveksthul@bluepinapple.com",
     description="",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```


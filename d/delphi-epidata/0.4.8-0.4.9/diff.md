# Comparing `tmp/delphi_epidata-0.4.8.tar.gz` & `tmp/delphi_epidata-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delphi_epidata-0.4.8.tar", last modified: Tue Apr  4 18:24:52 2023, max compression
+gzip compressed data, was "delphi_epidata-0.4.9.tar", last modified: Wed Apr  5 15:40:12 2023, max compression
```

## Comparing `delphi_epidata-0.4.8.tar` & `delphi_epidata-0.4.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:24:52.217341 delphi_epidata-0.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-04 18:24:40.000000 delphi_epidata-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-04 18:24:52.217341 delphi_epidata-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-04 18:24:40.000000 delphi_epidata-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:24:52.217341 delphi_epidata-0.4.8/delphi_epidata/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-04 18:24:40.000000 delphi_epidata-0.4.8/delphi_epidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24834 2023-04-04 18:24:51.000000 delphi_epidata-0.4.8/delphi_epidata/delphi_epidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 18:24:52.217341 delphi_epidata-0.4.8/delphi_epidata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-04 18:24:51.000000 delphi_epidata-0.4.8/delphi_epidata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-04 18:24:52.000000 delphi_epidata-0.4.8/delphi_epidata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 18:24:51.000000 delphi_epidata-0.4.8/delphi_epidata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-04 18:24:51.000000 delphi_epidata-0.4.8/delphi_epidata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-04 18:24:51.000000 delphi_epidata-0.4.8/delphi_epidata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 18:24:52.217341 delphi_epidata-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-04 18:24:40.000000 delphi_epidata-0.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:40:12.578888 delphi_epidata-0.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-04-05 15:40:02.000000 delphi_epidata-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-05 15:40:12.578888 delphi_epidata-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-05 15:40:02.000000 delphi_epidata-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:40:12.578888 delphi_epidata-0.4.9/delphi_epidata/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-05 15:40:02.000000 delphi_epidata-0.4.9/delphi_epidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24834 2023-04-05 15:40:11.000000 delphi_epidata-0.4.9/delphi_epidata/delphi_epidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 15:40:12.578888 delphi_epidata-0.4.9/delphi_epidata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-04-05 15:40:12.000000 delphi_epidata-0.4.9/delphi_epidata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-04-05 15:40:12.000000 delphi_epidata-0.4.9/delphi_epidata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 15:40:12.000000 delphi_epidata-0.4.9/delphi_epidata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-05 15:40:12.000000 delphi_epidata-0.4.9/delphi_epidata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-05 15:40:12.000000 delphi_epidata-0.4.9/delphi_epidata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 15:40:12.578888 delphi_epidata-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-04-05 15:40:02.000000 delphi_epidata-0.4.9/setup.py
```

### Comparing `delphi_epidata-0.4.8/LICENSE` & `delphi_epidata-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `delphi_epidata-0.4.8/PKG-INFO` & `delphi_epidata-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphi_epidata
-Version: 0.4.8
+Version: 0.4.9
 Summary: A programmatic interface to Delphi's Epidata API.
 Home-page: https://github.com/cmu-delphi/delphi-epidata
 Author: David Farrow
 Author-email: dfarrow0@gmail.com
 License: UNKNOWN
 Description: # Delphi Epidata API Client
```

### Comparing `delphi_epidata-0.4.8/delphi_epidata/delphi_epidata.py` & `delphi_epidata-0.4.9/delphi_epidata/delphi_epidata.py`

 * *Files identical despite different names*

### Comparing `delphi_epidata-0.4.8/delphi_epidata.egg-info/PKG-INFO` & `delphi_epidata-0.4.9/delphi_epidata.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delphi-epidata
-Version: 0.4.8
+Version: 0.4.9
 Summary: A programmatic interface to Delphi's Epidata API.
 Home-page: https://github.com/cmu-delphi/delphi-epidata
 Author: David Farrow
 Author-email: dfarrow0@gmail.com
 License: UNKNOWN
 Description: # Delphi Epidata API Client
```

### Comparing `delphi_epidata-0.4.8/setup.py` & `delphi_epidata-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="delphi_epidata",
-    version="0.4.8",
+    version="0.4.9",
     author="David Farrow",
     author_email="dfarrow0@gmail.com",
     description="A programmatic interface to Delphi's Epidata API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cmu-delphi/delphi-epidata",
     packages=setuptools.find_packages(),
```


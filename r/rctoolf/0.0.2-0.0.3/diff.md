# Comparing `tmp/rctoolf-0.0.2.tar.gz` & `tmp/rctoolf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rctoolf-0.0.2.tar", last modified: Fri Apr 14 09:16:29 2023, max compression
+gzip compressed data, was "rctoolf-0.0.3.tar", last modified: Wed Apr 19 08:29:32 2023, max compression
```

## Comparing `rctoolf-0.0.2.tar` & `rctoolf-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,16 @@
-drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 09:16:29.068453 rctoolf-0.0.2/
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1068 2023-04-14 08:22:53.000000 rctoolf-0.0.2/LICENSE
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 01:10:38.000000 rctoolf-0.0.2/MANIFEST.in
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1674 2023-04-14 09:16:29.068210 rctoolf-0.0.2/PKG-INFO
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        9 2023-04-14 09:14:57.000000 rctoolf-0.0.2/README.md
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)      584 2023-04-14 09:16:12.000000 rctoolf-0.0.2/pyproject.toml
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)       38 2023-04-14 09:16:29.068526 rctoolf-0.0.2/setup.cfg
-drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 09:16:29.064024 rctoolf-0.0.2/src/
-drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 09:16:29.066036 rctoolf-0.0.2/src/rctoolf/
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)       22 2023-04-14 01:14:19.000000 rctoolf-0.0.2/src/rctoolf/__init__.py
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1336 2023-04-14 00:35:51.000000 rctoolf-0.0.2/src/rctoolf/webhook.py
-drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 09:16:29.067821 rctoolf-0.0.2/src/rctoolf.egg-info/
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1674 2023-04-14 09:16:29.000000 rctoolf-0.0.2/src/rctoolf.egg-info/PKG-INFO
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)      265 2023-04-14 09:16:29.000000 rctoolf-0.0.2/src/rctoolf.egg-info/SOURCES.txt
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        1 2023-04-14 09:16:29.000000 rctoolf-0.0.2/src/rctoolf.egg-info/dependency_links.txt
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        5 2023-04-14 09:16:29.000000 rctoolf-0.0.2/src/rctoolf.egg-info/requires.txt
--rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        8 2023-04-14 09:16:29.000000 rctoolf-0.0.2/src/rctoolf.egg-info/top_level.txt
+drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-19 08:29:32.870358 rctoolf-0.0.3/
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1068 2023-04-14 08:22:53.000000 rctoolf-0.0.3/LICENSE
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-14 01:10:38.000000 rctoolf-0.0.3/MANIFEST.in
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1674 2023-04-19 08:29:32.869980 rctoolf-0.0.3/PKG-INFO
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        9 2023-04-14 09:14:57.000000 rctoolf-0.0.3/README.md
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)      572 2023-04-19 08:28:51.000000 rctoolf-0.0.3/pyproject.toml
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)       38 2023-04-19 08:29:32.870480 rctoolf-0.0.3/setup.cfg
+drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-19 08:29:32.866205 rctoolf-0.0.3/src/
+drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-19 08:29:32.868125 rctoolf-0.0.3/src/rctoolf/
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)       22 2023-04-19 08:28:58.000000 rctoolf-0.0.3/src/rctoolf/__init__.py
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1336 2023-04-14 00:35:51.000000 rctoolf-0.0.3/src/rctoolf/webhook.py
+drwxr-xr-x   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        0 2023-04-19 08:29:32.869410 rctoolf-0.0.3/src/rctoolf.egg-info/
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)     1674 2023-04-19 08:29:32.000000 rctoolf-0.0.3/src/rctoolf.egg-info/PKG-INFO
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)      231 2023-04-19 08:29:32.000000 rctoolf-0.0.3/src/rctoolf.egg-info/SOURCES.txt
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        1 2023-04-19 08:29:32.000000 rctoolf-0.0.3/src/rctoolf.egg-info/dependency_links.txt
+-rw-r--r--   0 glorin.li (1511914502) RCOFFICE\Domain Users (1800847059)        8 2023-04-19 08:29:32.000000 rctoolf-0.0.3/src/rctoolf.egg-info/top_level.txt
```

### Comparing `rctoolf-0.0.2/LICENSE` & `rctoolf-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rctoolf-0.0.2/PKG-INFO` & `rctoolf-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rctoolf
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for RC
 Author-email: Glorin Li <ligr1991@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rctoolf-0.0.2/pyproject.toml` & `rctoolf-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rctoolf"
-version = "0.0.2"
+version = "0.0.3"
 description = "Tools for RC"
 readme = "README.md"
 authors = [{ name = "Glorin Li", email = "ligr1991@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["rc", "webhook"]
-dependencies = [
-    "json"
-]
+dependencies = []
 requires-python = ">=3.0"
 
 [project.urls]
 Homepage = "https://github.com/glorinli/rctoolf"
```

### Comparing `rctoolf-0.0.2/src/rctoolf/webhook.py` & `rctoolf-0.0.3/src/rctoolf/webhook.py`

 * *Files identical despite different names*

### Comparing `rctoolf-0.0.2/src/rctoolf.egg-info/PKG-INFO` & `rctoolf-0.0.3/src/rctoolf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rctoolf
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for RC
 Author-email: Glorin Li <ligr1991@gmail.com>
 License: MIT License
         
         Copyright (c) [year] [fullname]
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


# Comparing `tmp/kiwigrad-0.17.tar.gz` & `tmp/kiwigrad-0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwigrad-0.17.tar", last modified: Mon Apr 17 22:31:47 2023, max compression
+gzip compressed data, was "kiwigrad-0.18.tar", last modified: Wed Apr 19 20:51:31 2023, max compression
```

## Comparing `kiwigrad-0.17.tar` & `kiwigrad-0.18.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-17 22:31:47.910502 kiwigrad-0.17/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.17/LICENSE
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.17/MANIFEST.in
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-17 22:31:47.909969 kiwigrad-0.17/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      177 2023-04-03 14:22:56.000000 kiwigrad-0.17/README.md
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-17 22:31:47.907831 kiwigrad-0.17/kiwigrad/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      193 2023-04-17 22:25:10.000000 kiwigrad-0.17/kiwigrad/__init__.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.17/kiwigrad/engine.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      970 2023-04-09 13:06:00.000000 kiwigrad-0.17/kiwigrad/graph.py
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     5514 2023-04-17 22:24:41.000000 kiwigrad-0.17/kiwigrad/nn.py
-drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-17 22:31:47.909442 kiwigrad-0.17/kiwigrad.egg-info/
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-17 22:31:47.000000 kiwigrad-0.17/kiwigrad.egg-info/PKG-INFO
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      276 2023-04-17 22:31:47.000000 kiwigrad-0.17/kiwigrad.egg-info/SOURCES.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-17 22:31:47.000000 kiwigrad-0.17/kiwigrad.egg-info/dependency_links.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-17 22:31:47.000000 kiwigrad-0.17/kiwigrad.egg-info/requires.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-17 22:31:47.000000 kiwigrad-0.17/kiwigrad.egg-info/top_level.txt
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      666 2023-04-17 22:24:58.000000 kiwigrad-0.17/pyproject.toml
--rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-17 22:31:47.910661 kiwigrad-0.17/setup.cfg
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-19 20:51:31.012167 kiwigrad-0.18/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1073 2022-11-30 14:22:32.000000 kiwigrad-0.18/LICENSE
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       22 2023-04-08 12:11:45.000000 kiwigrad-0.18/MANIFEST.in
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-19 20:51:31.011738 kiwigrad-0.18/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      177 2023-04-03 14:22:56.000000 kiwigrad-0.18/README.md
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-19 20:51:31.008570 kiwigrad-0.18/kiwigrad/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      289 2023-04-19 20:47:33.000000 kiwigrad-0.18/kiwigrad/__init__.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     4222 2023-04-09 13:04:30.000000 kiwigrad-0.18/kiwigrad/engine.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      970 2023-04-09 13:06:00.000000 kiwigrad-0.18/kiwigrad/graph.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1200 2023-04-19 20:42:21.000000 kiwigrad-0.18/kiwigrad/layers.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     3221 2023-04-19 20:49:44.000000 kiwigrad-0.18/kiwigrad/neurons.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1668 2023-04-19 20:50:24.000000 kiwigrad-0.18/kiwigrad/nn.py
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      144 2023-04-19 20:29:26.000000 kiwigrad-0.18/kiwigrad/skeleton.py
+drwxr-xr-x   0 marcosalvalaggio   (501) staff       (20)        0 2023-04-19 20:51:31.011194 kiwigrad-0.18/kiwigrad.egg-info/
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)     1933 2023-04-19 20:51:30.000000 kiwigrad-0.18/kiwigrad.egg-info/PKG-INFO
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      336 2023-04-19 20:51:31.000000 kiwigrad-0.18/kiwigrad.egg-info/SOURCES.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        1 2023-04-19 20:51:30.000000 kiwigrad-0.18/kiwigrad.egg-info/dependency_links.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-19 20:51:30.000000 kiwigrad-0.18/kiwigrad.egg-info/requires.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)        9 2023-04-19 20:51:30.000000 kiwigrad-0.18/kiwigrad.egg-info/top_level.txt
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)      666 2023-04-19 20:47:37.000000 kiwigrad-0.18/pyproject.toml
+-rw-r--r--   0 marcosalvalaggio   (501) staff       (20)       38 2023-04-19 20:51:31.012307 kiwigrad-0.18/setup.cfg
```

### Comparing `kiwigrad-0.17/LICENSE` & `kiwigrad-0.18/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.17/PKG-INFO` & `kiwigrad-0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.17
+Version: 0.18
 Summary: Mini deep learning framework
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `kiwigrad-0.17/kiwigrad/engine.py` & `kiwigrad-0.18/kiwigrad/engine.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.17/kiwigrad/graph.py` & `kiwigrad-0.18/kiwigrad/graph.py`

 * *Files identical despite different names*

### Comparing `kiwigrad-0.17/kiwigrad.egg-info/PKG-INFO` & `kiwigrad-0.18/kiwigrad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwigrad
-Version: 0.17
+Version: 0.18
 Summary: Mini deep learning framework
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `kiwigrad-0.17/pyproject.toml` & `kiwigrad-0.18/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "kiwigrad"
-version = "0.17"
+version = "0.18"
 authors = [
   { name="Marco Salvalaggio", email="mar.salvalaggio@gmail.com" },
 ]
 description = "Mini deep learning framework"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```


# Comparing `tmp/FPfits-0.0.2.tar.gz` & `tmp/FPfits-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FPfits-0.0.2.tar", last modified: Tue Apr 18 22:55:00 2023, max compression
+gzip compressed data, was "FPfits-0.0.3.tar", last modified: Tue Apr 18 22:56:35 2023, max compression
```

## Comparing `FPfits-0.0.2.tar` & `FPfits-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-04-18 22:55:00.530019 FPfits-0.0.2/
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-04-18 22:55:00.530019 FPfits-0.0.2/FPfits.egg-info/
--rw-rw-r--   0 felix     (1000) felix     (1000)      273 2023-04-18 22:55:00.000000 FPfits-0.0.2/FPfits.egg-info/PKG-INFO
--rw-rw-r--   0 felix     (1000) felix     (1000)      197 2023-04-18 22:55:00.000000 FPfits-0.0.2/FPfits.egg-info/SOURCES.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)        1 2023-04-18 22:55:00.000000 FPfits-0.0.2/FPfits.egg-info/dependency_links.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)       17 2023-04-18 22:55:00.000000 FPfits-0.0.2/FPfits.egg-info/requires.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)        8 2023-04-18 22:55:00.000000 FPfits-0.0.2/FPfits.egg-info/top_level.txt
--rw-rw-r--   0 felix     (1000) felix     (1000)      273 2023-04-18 22:55:00.530019 FPfits-0.0.2/PKG-INFO
-drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-04-18 22:55:00.530019 FPfits-0.0.2/fitting/
--rw-rw-r--   0 felix     (1000) felix     (1000)        0 2023-04-18 22:54:21.000000 FPfits-0.0.2/fitting/__init__.py
--rw-rw-r--   0 felix     (1000) felix     (1000)     3454 2023-04-18 22:16:03.000000 FPfits-0.0.2/fitting/plotting.py
--rw-rw-r--   0 felix     (1000) felix     (1000)       38 2023-04-18 22:55:00.530019 FPfits-0.0.2/setup.cfg
--rw-rw-r--   0 felix     (1000) felix     (1000)      471 2023-04-18 22:54:54.000000 FPfits-0.0.2/setup.py
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-04-18 22:56:35.901083 FPfits-0.0.3/
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-04-18 22:56:35.901083 FPfits-0.0.3/FPfits.egg-info/
+-rw-rw-r--   0 felix     (1000) felix     (1000)      273 2023-04-18 22:56:35.000000 FPfits-0.0.3/FPfits.egg-info/PKG-INFO
+-rw-rw-r--   0 felix     (1000) felix     (1000)      197 2023-04-18 22:56:35.000000 FPfits-0.0.3/FPfits.egg-info/SOURCES.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)        1 2023-04-18 22:56:35.000000 FPfits-0.0.3/FPfits.egg-info/dependency_links.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)       17 2023-04-18 22:56:35.000000 FPfits-0.0.3/FPfits.egg-info/requires.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)        8 2023-04-18 22:56:35.000000 FPfits-0.0.3/FPfits.egg-info/top_level.txt
+-rw-rw-r--   0 felix     (1000) felix     (1000)      273 2023-04-18 22:56:35.901083 FPfits-0.0.3/PKG-INFO
+drwxrwxr-x   0 felix     (1000) felix     (1000)        0 2023-04-18 22:56:35.901083 FPfits-0.0.3/fitting/
+-rw-rw-r--   0 felix     (1000) felix     (1000)        0 2023-04-18 22:54:21.000000 FPfits-0.0.3/fitting/__init__.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)     3497 2023-04-18 22:56:05.000000 FPfits-0.0.3/fitting/plotting.py
+-rw-rw-r--   0 felix     (1000) felix     (1000)       38 2023-04-18 22:56:35.901083 FPfits-0.0.3/setup.cfg
+-rw-rw-r--   0 felix     (1000) felix     (1000)      471 2023-04-18 22:56:24.000000 FPfits-0.0.3/setup.py
```

### Comparing `FPfits-0.0.2/fitting/plotting.py` & `FPfits-0.0.3/fitting/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,14 +107,16 @@
         
             
             
         
     
 
 
+def add_one(number):
+    return number + 1
 
 
 
 
 
 
 xdata = unp.uarray([1,2,3,4],[0.1]*4)
```


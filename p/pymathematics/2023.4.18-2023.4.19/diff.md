# Comparing `tmp/pymathematics-2023.4.18.tar.gz` & `tmp/pymathematics-2023.4.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymathematics-2023.4.18.tar", last modified: Tue Apr 18 13:18:36 2023, max compression
+gzip compressed data, was "pymathematics-2023.4.19.tar", last modified: Wed Apr 19 10:26:51 2023, max compression
```

## Comparing `pymathematics-2023.4.18.tar` & `pymathematics-2023.4.19.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-18 13:18:36.387120 pymathematics-2023.4.18/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.18/LICENSE
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-18 13:18:36.377117 pymathematics-2023.4.18/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       28 2023-04-18 13:11:32.000000 pymathematics-2023.4.18/README.md
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-18 13:18:35.955893 pymathematics-2023.4.18/pymathematics/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    12206 2023-04-18 13:11:37.000000 pymathematics-2023.4.18/pymathematics/__init__.py
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-18 13:11:26.000000 pymathematics-2023.4.18/pymathematics/info.py
-drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-18 13:18:36.306120 pymathematics-2023.4.18/pymathematics.egg-info/
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-18 13:18:33.000000 pymathematics-2023.4.18/pymathematics.egg-info/PKG-INFO
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-18 13:18:33.000000 pymathematics-2023.4.18/pymathematics.egg-info/SOURCES.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-18 13:18:33.000000 pymathematics-2023.4.18/pymathematics.egg-info/dependency_links.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-18 13:18:33.000000 pymathematics-2023.4.18/pymathematics.egg-info/top_level.txt
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-18 13:18:36.391119 pymathematics-2023.4.18/setup.cfg
--rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-18 13:12:28.000000 pymathematics-2023.4.18/setup.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-19 10:26:51.024355 pymathematics-2023.4.19/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)     1088 2023-04-16 06:03:02.000000 pymathematics-2023.4.19/LICENSE
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-19 10:26:50.997290 pymathematics-2023.4.19/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       27 2023-04-18 17:29:05.000000 pymathematics-2023.4.19/README.md
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-19 10:26:50.463290 pymathematics-2023.4.19/pymathematics/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)    14568 2023-04-19 09:30:51.000000 pymathematics-2023.4.19/pymathematics/__init__.py
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      111 2023-04-18 17:28:53.000000 pymathematics-2023.4.19/pymathematics/info.py
+drwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        0 2023-04-19 10:26:50.797290 pymathematics-2023.4.19/pymathematics.egg-info/
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      507 2023-04-19 10:26:47.000000 pymathematics-2023.4.19/pymathematics.egg-info/PKG-INFO
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      222 2023-04-19 10:26:47.000000 pymathematics-2023.4.19/pymathematics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)        1 2023-04-19 10:26:47.000000 pymathematics-2023.4.19/pymathematics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       14 2023-04-19 10:26:47.000000 pymathematics-2023.4.19/pymathematics.egg-info/top_level.txt
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)       38 2023-04-19 10:26:51.027291 pymathematics-2023.4.19/setup.cfg
+-rwxrwxrwx   0 sahil-rajwar  (1000) sahil-rajwar  (1000)      689 2023-04-18 17:29:00.000000 pymathematics-2023.4.19/setup.py
```

### Comparing `pymathematics-2023.4.18/LICENSE` & `pymathematics-2023.4.19/LICENSE`

 * *Files identical despite different names*

### Comparing `pymathematics-2023.4.18/setup.py` & `pymathematics-2023.4.19/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup,find_packages
 
 setup(
     name = "pymathematics",
-    version = "2023.4.18",
+    version = "2023.4.19",
     description = "package for mathematics",
     long_description = "for more info, check the github repository",
     author = "Sahil Rajwar",
     maintainer = "its_Sahil",
     author_email = "justsahilrajwar2004@gmail.com",
     packages = ["pymathematics"],
     license = "MIT",
```


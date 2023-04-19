# Comparing `tmp/buge-0.0.3.tar.gz` & `tmp/buge-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buge-0.0.3.tar", last modified: Tue Apr 18 02:32:29 2023, max compression
+gzip compressed data, was "buge-0.0.4.tar", last modified: Wed Apr 19 01:19:38 2023, max compression
```

## Comparing `buge-0.0.3.tar` & `buge-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-18 02:32:29.912489 buge-0.0.3/
--rw-r--r--   0 damonpickett   (501) staff       (20)     1073 2023-04-14 22:43:18.000000 buge-0.0.3/LICENSE
--rw-r--r--   0 damonpickett   (501) staff       (20)       25 2023-04-14 22:43:29.000000 buge-0.0.3/MANIFEST.in
--rw-r--r--   0 damonpickett   (501) staff       (20)      637 2023-04-18 02:32:29.912531 buge-0.0.3/PKG-INFO
--rw-r--r--   0 damonpickett   (501) staff       (20)        0 2023-04-14 22:43:42.000000 buge-0.0.3/README.md
-drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-18 02:32:29.911628 buge-0.0.3/buge/
--rw-r--r--   0 damonpickett   (501) staff       (20)     2028 2023-04-18 02:30:28.000000 buge-0.0.3/buge/main.py
-drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-18 02:32:29.912393 buge-0.0.3/buge.egg-info/
--rw-r--r--   0 damonpickett   (501) staff       (20)      637 2023-04-18 02:32:29.000000 buge-0.0.3/buge.egg-info/PKG-INFO
--rw-r--r--   0 damonpickett   (501) staff       (20)      246 2023-04-18 02:32:29.000000 buge-0.0.3/buge.egg-info/SOURCES.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)        1 2023-04-18 02:32:29.000000 buge-0.0.3/buge.egg-info/dependency_links.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)       40 2023-04-18 02:32:29.000000 buge-0.0.3/buge.egg-info/entry_points.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)       26 2023-04-18 02:32:29.000000 buge-0.0.3/buge.egg-info/requires.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)        5 2023-04-18 02:32:29.000000 buge-0.0.3/buge.egg-info/top_level.txt
--rw-r--r--   0 damonpickett   (501) staff       (20)      644 2023-04-18 02:30:40.000000 buge-0.0.3/pyproject.toml
--rw-r--r--   0 damonpickett   (501) staff       (20)      784 2023-04-18 02:32:29.912764 buge-0.0.3/setup.cfg
--rw-r--r--   0 damonpickett   (501) staff       (20)       37 2023-04-13 22:46:26.000000 buge-0.0.3/setup.py
+drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-19 01:19:38.121640 buge-0.0.4/
+-rw-r--r--   0 damonpickett   (501) staff       (20)     1073 2023-04-14 22:43:18.000000 buge-0.0.4/LICENSE
+-rw-r--r--   0 damonpickett   (501) staff       (20)       25 2023-04-14 22:43:29.000000 buge-0.0.4/MANIFEST.in
+-rw-r--r--   0 damonpickett   (501) staff       (20)     3863 2023-04-19 01:19:38.121690 buge-0.0.4/PKG-INFO
+-rw-r--r--   0 damonpickett   (501) staff       (20)     3224 2023-04-19 01:18:42.000000 buge-0.0.4/README.md
+drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-19 01:19:38.120695 buge-0.0.4/buge/
+-rw-r--r--   0 damonpickett   (501) staff       (20)     2988 2023-04-19 01:18:42.000000 buge-0.0.4/buge/main.py
+drwxr-xr-x   0 damonpickett   (501) staff       (20)        0 2023-04-19 01:19:38.121510 buge-0.0.4/buge.egg-info/
+-rw-r--r--   0 damonpickett   (501) staff       (20)     3863 2023-04-19 01:19:38.000000 buge-0.0.4/buge.egg-info/PKG-INFO
+-rw-r--r--   0 damonpickett   (501) staff       (20)      246 2023-04-19 01:19:38.000000 buge-0.0.4/buge.egg-info/SOURCES.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)        1 2023-04-19 01:19:38.000000 buge-0.0.4/buge.egg-info/dependency_links.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)       40 2023-04-19 01:19:38.000000 buge-0.0.4/buge.egg-info/entry_points.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)       26 2023-04-19 01:19:38.000000 buge-0.0.4/buge.egg-info/requires.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)        5 2023-04-19 01:19:38.000000 buge-0.0.4/buge.egg-info/top_level.txt
+-rw-r--r--   0 damonpickett   (501) staff       (20)      644 2023-04-19 01:19:09.000000 buge-0.0.4/pyproject.toml
+-rw-r--r--   0 damonpickett   (501) staff       (20)      784 2023-04-19 01:19:38.121931 buge-0.0.4/setup.cfg
+-rw-r--r--   0 damonpickett   (501) staff       (20)       37 2023-04-13 22:46:26.000000 buge-0.0.4/setup.py
```

### Comparing `buge-0.0.3/LICENSE` & `buge-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `buge-0.0.3/pyproject.toml` & `buge-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "buge"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Damon Pickett", email="damon.pickett@gmail.com" },
 ]
 description = "buge is a command-line application that uses the OpenAI API to diagnose bugs when programming."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `buge-0.0.3/setup.cfg` & `buge-0.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = buge
-version = 0.0.3
+version = 0.0.4
 author = Damon Pickett
 author_email = damon.pickett@gmail.com
 description = buge is a command-line application that uses the OpenAI API to diagnose bugs when programming.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/damonpickett/buge
 classifiers =
```


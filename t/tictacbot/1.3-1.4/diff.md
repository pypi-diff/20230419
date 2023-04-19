# Comparing `tmp/tictacbot-1.3.tar.gz` & `tmp/tictacbot-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tictacbot-1.3.tar", last modified: Wed Apr 19 19:24:18 2023, max compression
+gzip compressed data, was "tictacbot-1.4.tar", last modified: Wed Apr 19 19:30:10 2023, max compression
```

## Comparing `tictacbot-1.3.tar` & `tictacbot-1.4.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 19:24:18.659832 tictacbot-1.3/
--rw-r--r--   0 edgarcresson   (501) staff       (20)      234 2023-04-19 19:24:18.659700 tictacbot-1.3/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)       84 2023-04-19 15:56:47.000000 tictacbot-1.3/README.md
--rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-19 19:24:18.659880 tictacbot-1.3/setup.cfg
--rw-r--r--   0 edgarcresson   (501) staff       (20)      571 2023-04-19 19:23:10.000000 tictacbot-1.3/setup.py
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 19:24:18.658538 tictacbot-1.3/tictacbot/
--rw-r--r--   0 edgarcresson   (501) staff       (20)     6363 2023-04-19 19:23:25.000000 tictacbot-1.3/tictacbot/listen.py
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 19:24:18.659531 tictacbot-1.3/tictacbot.egg-info/
--rw-r--r--   0 edgarcresson   (501) staff       (20)      234 2023-04-19 19:24:18.000000 tictacbot-1.3/tictacbot.egg-info/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)      238 2023-04-19 19:24:18.000000 tictacbot-1.3/tictacbot.egg-info/SOURCES.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-19 19:24:18.000000 tictacbot-1.3/tictacbot.egg-info/dependency_links.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-19 19:24:18.000000 tictacbot-1.3/tictacbot.egg-info/entry_points.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-19 19:24:18.000000 tictacbot-1.3/tictacbot.egg-info/requires.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-19 19:24:18.000000 tictacbot-1.3/tictacbot.egg-info/top_level.txt
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 19:30:10.620500 tictacbot-1.4/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 tictacbot-1.4/MANIFEST.in
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      234 2023-04-19 19:30:10.620344 tictacbot-1.4/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       84 2023-04-19 15:56:47.000000 tictacbot-1.4/README.md
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-19 19:30:10.620542 tictacbot-1.4/setup.cfg
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      571 2023-04-19 19:29:50.000000 tictacbot-1.4/setup.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 19:30:10.619390 tictacbot-1.4/tictacbot/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-14 12:45:16.000000 tictacbot-1.4/tictacbot/gutenberg.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     6363 2023-04-19 19:23:25.000000 tictacbot-1.4/tictacbot/listen.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 19:30:10.620156 tictacbot-1.4/tictacbot.egg-info/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      234 2023-04-19 19:30:10.000000 tictacbot-1.4/tictacbot.egg-info/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      274 2023-04-19 19:30:10.000000 tictacbot-1.4/tictacbot.egg-info/SOURCES.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-19 19:30:10.000000 tictacbot-1.4/tictacbot.egg-info/dependency_links.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-19 19:30:10.000000 tictacbot-1.4/tictacbot.egg-info/entry_points.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-19 19:30:10.000000 tictacbot-1.4/tictacbot.egg-info/requires.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-19 19:30:10.000000 tictacbot-1.4/tictacbot.egg-info/top_level.txt
```

### Comparing `tictacbot-1.3/setup.py` & `tictacbot-1.4/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="tictacbot",
-    version="1.3",
+    version="1.4",
     packages=["tictacbot"],
     description="A program that makes you unbeatable at BombParty",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "pynput",
         "pyperclip",
```

### Comparing `tictacbot-1.3/tictacbot/listen.py` & `tictacbot-1.4/tictacbot/listen.py`

 * *Files identical despite different names*


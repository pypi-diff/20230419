# Comparing `tmp/pytictacbot-1.0.tar.gz` & `tmp/pytictacbot-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytictacbot-1.0.tar", last modified: Wed Apr 19 20:56:58 2023, max compression
+gzip compressed data, was "pytictacbot-1.1.tar", last modified: Wed Apr 19 21:05:54 2023, max compression
```

## Comparing `pytictacbot-1.0.tar` & `pytictacbot-1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 20:56:58.442736 pytictacbot-1.0/
--rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.0/MANIFEST.in
--rw-r--r--   0 edgarcresson   (501) staff       (20)      236 2023-04-19 20:56:58.442574 pytictacbot-1.0/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)       84 2023-04-19 15:56:47.000000 pytictacbot-1.0/README.md
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 20:56:58.438740 pytictacbot-1.0/pytictacbot.egg-info/
--rw-r--r--   0 edgarcresson   (501) staff       (20)      236 2023-04-19 20:56:58.000000 pytictacbot-1.0/pytictacbot.egg-info/PKG-INFO
--rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-19 20:56:58.000000 pytictacbot-1.0/pytictacbot.egg-info/SOURCES.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-19 20:56:58.000000 pytictacbot-1.0/pytictacbot.egg-info/dependency_links.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-19 20:56:58.000000 pytictacbot-1.0/pytictacbot.egg-info/entry_points.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-19 20:56:58.000000 pytictacbot-1.0/pytictacbot.egg-info/requires.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-19 20:56:58.000000 pytictacbot-1.0/pytictacbot.egg-info/top_level.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-19 20:56:58.442780 pytictacbot-1.0/setup.cfg
--rw-r--r--   0 edgarcresson   (501) staff       (20)      573 2023-04-19 20:56:45.000000 pytictacbot-1.0/setup.py
-drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 20:56:58.442201 pytictacbot-1.0/tictacbot/
--rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-14 12:45:16.000000 pytictacbot-1.0/tictacbot/gutenberg.txt
--rw-r--r--   0 edgarcresson   (501) staff       (20)     6363 2023-04-19 19:37:00.000000 pytictacbot-1.0/tictacbot/listen.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 21:05:54.448773 pytictacbot-1.1/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       32 2023-04-19 19:29:28.000000 pytictacbot-1.1/MANIFEST.in
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      236 2023-04-19 21:05:54.448634 pytictacbot-1.1/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       84 2023-04-19 15:56:47.000000 pytictacbot-1.1/README.md
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 21:05:54.444871 pytictacbot-1.1/pytictacbot.egg-info/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      236 2023-04-19 21:05:54.000000 pytictacbot-1.1/pytictacbot.egg-info/PKG-INFO
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      286 2023-04-19 21:05:54.000000 pytictacbot-1.1/pytictacbot.egg-info/SOURCES.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)        1 2023-04-19 21:05:54.000000 pytictacbot-1.1/pytictacbot.egg-info/dependency_links.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       56 2023-04-19 21:05:54.000000 pytictacbot-1.1/pytictacbot.egg-info/entry_points.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       40 2023-04-19 21:05:54.000000 pytictacbot-1.1/pytictacbot.egg-info/requires.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       10 2023-04-19 21:05:54.000000 pytictacbot-1.1/pytictacbot.egg-info/top_level.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)       38 2023-04-19 21:05:54.448811 pytictacbot-1.1/setup.cfg
+-rw-r--r--   0 edgarcresson   (501) staff       (20)      604 2023-04-19 21:05:48.000000 pytictacbot-1.1/setup.py
+drwxr-xr-x   0 edgarcresson   (501) staff       (20)        0 2023-04-19 21:05:54.448409 pytictacbot-1.1/tictacbot/
+-rw-r--r--   0 edgarcresson   (501) staff       (20)  3895958 2023-04-14 12:45:16.000000 pytictacbot-1.1/tictacbot/gutenberg.txt
+-rw-r--r--   0 edgarcresson   (501) staff       (20)     6363 2023-04-19 19:37:00.000000 pytictacbot-1.1/tictacbot/listen.py
```

### Comparing `pytictacbot-1.0/setup.py` & `pytictacbot-1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pytictacbot",
-    version="1.0",
+    version="1.1",
     packages=["tictacbot"],
+    include_package_data=True,
     description="A program that makes you unbeatable at BombParty",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         "pynput",
         "pyperclip",
         "pyautogui",
```

### Comparing `pytictacbot-1.0/tictacbot/gutenberg.txt` & `pytictacbot-1.1/tictacbot/gutenberg.txt`

 * *Files identical despite different names*

### Comparing `pytictacbot-1.0/tictacbot/listen.py` & `pytictacbot-1.1/tictacbot/listen.py`

 * *Files identical despite different names*


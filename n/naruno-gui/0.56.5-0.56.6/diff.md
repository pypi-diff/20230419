# Comparing `tmp/naruno_gui-0.56.5.tar.gz` & `tmp/naruno_gui-0.56.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_gui-0.56.5.tar", last modified: Tue Apr 18 15:16:30 2023, max compression
+gzip compressed data, was "naruno_gui-0.56.6.tar", last modified: Tue Apr 18 23:57:25 2023, max compression
```

## Comparing `naruno_gui-0.56.5.tar` & `naruno_gui-0.56.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:16:30.027656 naruno_gui-0.56.5/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-18 15:16:30.027656 naruno_gui-0.56.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:16:30.027656 naruno_gui-0.56.5/naruno_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-18 15:16:29.000000 naruno_gui-0.56.5/naruno_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-18 15:16:30.000000 naruno_gui-0.56.5/naruno_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:16:29.000000 naruno_gui-0.56.5/naruno_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:16:29.000000 naruno_gui-0.56.5/naruno_gui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-18 15:16:29.000000 naruno_gui-0.56.5/naruno_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:16:29.000000 naruno_gui-0.56.5/naruno_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:16:30.027656 naruno_gui-0.56.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-18 15:16:12.000000 naruno_gui-0.56.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:57:25.605048 naruno_gui-0.56.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-18 23:57:25.605048 naruno_gui-0.56.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:57:25.605048 naruno_gui-0.56.6/naruno_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-18 23:57:25.000000 naruno_gui-0.56.6/naruno_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-18 23:57:25.000000 naruno_gui-0.56.6/naruno_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:57:25.000000 naruno_gui-0.56.6/naruno_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:57:25.000000 naruno_gui-0.56.6/naruno_gui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-18 23:57:25.000000 naruno_gui-0.56.6/naruno_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:57:25.000000 naruno_gui-0.56.6/naruno_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 23:57:25.605048 naruno_gui-0.56.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-18 23:57:07.000000 naruno_gui-0.56.6/setup.py
```

### Comparing `naruno_gui-0.56.5/setup.py` & `naruno_gui-0.56.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from setuptools import setup
 
 setup(
     name="naruno_gui",
-    version="0.56.5",
+    version="0.56.6",
     description="""This is GUI mode installer for Naruno""",
     url="https://docs.naruno.org/",
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     license="MPL-2.0",
     install_requires="""
 Kivy==2.1.0
```


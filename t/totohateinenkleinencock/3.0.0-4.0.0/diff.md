# Comparing `tmp/totohateinenkleinencock-3.0.0.tar.gz` & `tmp/totohateinenkleinencock-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totohateinenkleinencock-3.0.0.tar", last modified: Wed Apr 19 17:54:44 2023, max compression
+gzip compressed data, was "totohateinenkleinencock-4.0.0.tar", last modified: Wed Apr 19 17:59:06 2023, max compression
```

## Comparing `totohateinenkleinencock-3.0.0.tar` & `totohateinenkleinencock-4.0.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:54:44.784672 totohateinenkleinencock-3.0.0/
--rw-r--r--   0 root         (0) root         (0)      320 2023-04-19 17:54:44.784672 totohateinenkleinencock-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 17:54:44.784672 totohateinenkleinencock-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      533 2023-04-19 17:54:43.000000 totohateinenkleinencock-3.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:54:44.780672 totohateinenkleinencock-3.0.0/totohateinenkleinencock/
--rw-r--r--   0 root         (0) root         (0)    82231 2023-04-19 17:54:44.000000 totohateinenkleinencock-3.0.0/totohateinenkleinencock/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:54:44.784672 totohateinenkleinencock-3.0.0/totohateinenkleinencock.egg-info/
--rw-r--r--   0 root         (0) root         (0)      320 2023-04-19 17:54:44.000000 totohateinenkleinencock-3.0.0/totohateinenkleinencock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      232 2023-04-19 17:54:44.000000 totohateinenkleinencock-3.0.0/totohateinenkleinencock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 17:54:44.000000 totohateinenkleinencock-3.0.0/totohateinenkleinencock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-19 17:54:44.000000 totohateinenkleinencock-3.0.0/totohateinenkleinencock.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:59:06.646238 totohateinenkleinencock-4.0.0/
+-rw-r--r--   0 root         (0) root         (0)      320 2023-04-19 17:59:06.646238 totohateinenkleinencock-4.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-19 17:59:06.646238 totohateinenkleinencock-4.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      533 2023-04-19 17:59:05.000000 totohateinenkleinencock-4.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:59:06.646238 totohateinenkleinencock-4.0.0/totohateinenkleinencock/
+-rw-r--r--   0 root         (0) root         (0)    82231 2023-04-19 17:59:06.000000 totohateinenkleinencock-4.0.0/totohateinenkleinencock/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 17:59:06.646238 totohateinenkleinencock-4.0.0/totohateinenkleinencock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      320 2023-04-19 17:59:06.000000 totohateinenkleinencock-4.0.0/totohateinenkleinencock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      232 2023-04-19 17:59:06.000000 totohateinenkleinencock-4.0.0/totohateinenkleinencock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 17:59:06.000000 totohateinenkleinencock-4.0.0/totohateinenkleinencock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-19 17:59:06.000000 totohateinenkleinencock-4.0.0/totohateinenkleinencock.egg-info/top_level.txt
```

### Comparing `totohateinenkleinencock-3.0.0/setup.py` & `totohateinenkleinencock-4.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '3.0.0'
+VERSION = '4.0.0'
 DESCRIPTION = "toto"
 LONG_DESCRIPTION = "toto"
 
 # Setting up
 setup(
     name="totohateinenkleinencock",
     version=VERSION,
```

### Comparing `totohateinenkleinencock-3.0.0/totohateinenkleinencock/__init__.py` & `totohateinenkleinencock-4.0.0/totohateinenkleinencock/__init__.py`

 * *Files identical despite different names*


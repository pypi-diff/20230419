# Comparing `tmp/badgie-0.4.0.tar.gz` & `tmp/badgie-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "badgie-0.4.0.tar", last modified: Sun Apr 16 06:56:54 2023, max compression
+gzip compressed data, was "badgie-0.5.0.tar", last modified: Wed Apr 19 05:24:19 2023, max compression
```

## Comparing `badgie-0.4.0.tar` & `badgie-0.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.968898 badgie-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-16 06:56:51.000000 badgie-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3936 2023-04-16 06:56:54.968898 badgie-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3044 2023-04-16 06:56:51.000000 badgie-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.962897 badgie-0.4.0/badgie/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-16 06:56:52.000000 badgie-0.4.0/badgie/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.966898 badgie-0.4.0/badgie/badges/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/badges/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/badges/_base.py
--rw-rw-rw-   0 root         (0) root         (0)      997 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/badges/brettops.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/badges/codestyle.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/badges/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)      511 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/badges/precommit.py
--rw-rw-rw-   0 root         (0) root         (0)     5154 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/cli.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.966898 badgie-0.4.0/badgie/detectors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/detectors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/detectors/precommit.py
--rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1524 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/parser.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.967898 badgie-0.4.0/badgie/providers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/providers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1432 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/providers/gitlab.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.967898 badgie-0.4.0/badgie/sources/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      749 2023-04-16 06:56:51.000000 badgie-0.4.0/badgie/sources/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-16 06:56:54.964897 badgie-0.4.0/badgie.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3936 2023-04-16 06:56:54.000000 badgie-0.4.0/badgie.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      677 2023-04-16 06:56:54.000000 badgie-0.4.0/badgie.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-16 06:56:54.000000 badgie-0.4.0/badgie.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-16 06:56:54.000000 badgie-0.4.0/badgie.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-04-16 06:56:54.000000 badgie-0.4.0/badgie.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-16 06:56:54.000000 badgie-0.4.0/badgie.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-16 06:56:54.969898 badgie-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1429 2023-04-16 06:56:52.000000 badgie-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.548009 badgie-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-04-19 05:24:15.000000 badgie-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3936 2023-04-19 05:24:19.548009 badgie-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3044 2023-04-19 05:24:15.000000 badgie-0.5.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.542008 badgie-0.5.0/badgie/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-19 05:24:16.000000 badgie-0.5.0/badgie/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.546009 badgie-0.5.0/badgie/badges/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/badges/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/badges/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)      997 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/badges/brettops.py
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/badges/codestyle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/badges/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)      494 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/badges/precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)     5154 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.547009 badgie-0.5.0/badgie/detectors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/detectors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1567 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/detectors/precommit.py
+-rw-rw-rw-   0 root         (0) root         (0)      368 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1524 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/parser.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.547009 badgie-0.5.0/badgie/providers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/providers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1432 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/providers/gitlab.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.548009 badgie-0.5.0/badgie/sources/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      749 2023-04-19 05:24:15.000000 badgie-0.5.0/badgie/sources/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-19 05:24:19.544009 badgie-0.5.0/badgie.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3936 2023-04-19 05:24:19.000000 badgie-0.5.0/badgie.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      677 2023-04-19 05:24:19.000000 badgie-0.5.0/badgie.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 05:24:19.000000 badgie-0.5.0/badgie.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-19 05:24:19.000000 badgie-0.5.0/badgie.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-19 05:24:19.000000 badgie-0.5.0/badgie.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-04-19 05:24:19.000000 badgie-0.5.0/badgie.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-04-19 05:24:19.549009 badgie-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1429 2023-04-19 05:24:16.000000 badgie-0.5.0/setup.py
```

### Comparing `badgie-0.4.0/LICENSE` & `badgie-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `badgie-0.4.0/PKG-INFO` & `badgie-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.4.0
+Version: 0.5.0
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge template markdown
 Platform: UNKNOWN
```

### Comparing `badgie-0.4.0/README.md` & `badgie-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `badgie-0.4.0/badgie/badges/_base.py` & `badgie-0.5.0/badgie/badges/_base.py`

 * *Files identical despite different names*

### Comparing `badgie-0.4.0/badgie/badges/brettops.py` & `badgie-0.5.0/badgie/badges/brettops.py`

 * *Files identical despite different names*

### Comparing `badgie-0.4.0/badgie/badges/codestyle.py` & `badgie-0.5.0/badgie/badges/codestyle.py`

 * *Files identical despite different names*

### Comparing `badgie-0.4.0/badgie/badges/gitlab.py` & `badgie-0.5.0/badgie/badges/gitlab.py`

 * *Files identical despite different names*

### Comparing `badgie-0.4.0/badgie/cli.py` & `badgie-0.5.0/badgie/cli.py`

 * *Files identical despite different names*

### Comparing `badgie-0.4.0/badgie/detectors/precommit.py` & `badgie-0.5.0/badgie/detectors/precommit.py`

 * *Files identical despite different names*

### Comparing `badgie-0.4.0/badgie/parser.py` & `badgie-0.5.0/badgie/parser.py`

 * *Files identical despite different names*

### Comparing `badgie-0.4.0/badgie/providers/gitlab.py` & `badgie-0.5.0/badgie/providers/gitlab.py`

 * *Files identical despite different names*

### Comparing `badgie-0.4.0/badgie/sources/base.py` & `badgie-0.5.0/badgie/sources/base.py`

 * *Files identical despite different names*

### Comparing `badgie-0.4.0/badgie.egg-info/PKG-INFO` & `badgie-0.5.0/badgie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: badgie
-Version: 0.4.0
+Version: 0.5.0
 Summary: Add all the badges with Badgie!
 Home-page: https://gitlab.com/brettops/tools/badgie
 Author: Brett Weir
 Author-email: brett@brettops.io
 License: MIT
 Keywords: badge template markdown
 Platform: UNKNOWN
```

### Comparing `badgie-0.4.0/badgie.egg-info/SOURCES.txt` & `badgie-0.5.0/badgie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `badgie-0.4.0/setup.py` & `badgie-0.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import find_packages, setup
 
 # injected version
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 # markdown readme
 long_description = open("README.md").read()
 
 # read requirements from requirements.in
 install_requires = open("requirements.in").read().splitlines()
```


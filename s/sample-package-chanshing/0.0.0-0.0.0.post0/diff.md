# Comparing `tmp/sample-package-chanshing-0.0.0.tar.gz` & `tmp/sample-package-chanshing-0.0.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sample-package-chanshing-0.0.0.tar", last modified: Tue Apr 18 18:19:13 2023, max compression
+gzip compressed data, was "sample-package-chanshing-0.0.0.post0.tar", last modified: Wed Apr 19 20:47:03 2023, max compression
```

## Comparing `sample-package-chanshing-0.0.0.tar` & `sample-package-chanshing-0.0.0.post0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:19:13.283439 sample-package-chanshing-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 18:19:03.000000 sample-package-chanshing-0.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-18 18:19:13.283439 sample-package-chanshing-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 18:19:03.000000 sample-package-chanshing-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-04-18 18:19:03.000000 sample-package-chanshing-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 18:19:13.283439 sample-package-chanshing-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-04-18 18:19:03.000000 sample-package-chanshing-0.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:19:13.279439 sample-package-chanshing-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:19:13.283439 sample-package-chanshing-0.0.0/src/sample_package/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-18 18:19:03.000000 sample-package-chanshing-0.0.0/src/sample_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-18 18:19:13.283439 sample-package-chanshing-0.0.0/src/sample_package/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 18:19:03.000000 sample-package-chanshing-0.0.0/src/sample_package/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 18:19:13.283439 sample-package-chanshing-0.0.0/src/sample_package_chanshing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-18 18:19:13.000000 sample-package-chanshing-0.0.0/src/sample_package_chanshing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-18 18:19:13.000000 sample-package-chanshing-0.0.0/src/sample_package_chanshing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 18:19:13.000000 sample-package-chanshing-0.0.0/src/sample_package_chanshing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-18 18:19:13.000000 sample-package-chanshing-0.0.0/src/sample_package_chanshing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-18 18:19:13.000000 sample-package-chanshing-0.0.0/src/sample_package_chanshing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 18:19:13.000000 sample-package-chanshing-0.0.0/src/sample_package_chanshing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-18 18:19:03.000000 sample-package-chanshing-0.0.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/src/sample_package/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/src/sample_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/src/sample_package/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/src/sample_package/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:47:03.777175 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-19 20:47:03.000000 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-19 20:47:03.000000 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:47:03.000000 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-19 20:47:03.000000 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-19 20:47:03.000000 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 20:47:03.000000 sample-package-chanshing-0.0.0.post0/src/sample_package_chanshing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-04-19 20:46:53.000000 sample-package-chanshing-0.0.0.post0/versioneer.py
```

### Comparing `sample-package-chanshing-0.0.0/pyproject.toml` & `sample-package-chanshing-0.0.0.post0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sample-package-chanshing-0.0.0/setup.py` & `sample-package-chanshing-0.0.0.post0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
+import sys
+import os.path
+# https://github.com/python-versioneer/python-versioneer/issues/193
+sys.path.insert(0, os.path.dirname(__file__))
+
 from setuptools import setup, find_packages
 import codecs
-import os.path
 
 import versioneer
 
 
 
 def main():
```

### Comparing `sample-package-chanshing-0.0.0/versioneer.py` & `sample-package-chanshing-0.0.0.post0/versioneer.py`

 * *Files identical despite different names*


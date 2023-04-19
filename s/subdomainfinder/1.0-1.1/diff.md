# Comparing `tmp/subdomainfinder-1.0.tar.gz` & `tmp/subdomainfinder-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subdomainfinder-1.0.tar", last modified: Wed Apr 19 19:44:21 2023, max compression
+gzip compressed data, was "subdomainfinder-1.1.tar", last modified: Wed Apr 19 20:10:26 2023, max compression
```

## Comparing `subdomainfinder-1.0.tar` & `subdomainfinder-1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwx------   0 u0_a189  (10189) u0_a189  (10189)        0 2023-04-19 19:44:21.105066 subdomainfinder-1.0/
--rw-------   0 u0_a189  (10189) u0_a189  (10189)     1792 2023-04-19 19:44:21.105066 subdomainfinder-1.0/PKG-INFO
--rw-------   0 u0_a189  (10189) u0_a189  (10189)      984 2023-04-19 19:02:43.000000 subdomainfinder-1.0/README.md
--rw-------   0 u0_a189  (10189) u0_a189  (10189)       38 2023-04-19 19:44:21.105066 subdomainfinder-1.0/setup.cfg
--rw-------   0 u0_a189  (10189) u0_a189  (10189)     1217 2023-04-19 19:43:53.000000 subdomainfinder-1.0/setup.py
-drwx------   0 u0_a189  (10189) u0_a189  (10189)        0 2023-04-19 19:44:21.101733 subdomainfinder-1.0/subdomainfinder/
--rw-------   0 u0_a189  (10189) u0_a189  (10189)     6137 2023-04-19 18:46:46.000000 subdomainfinder-1.0/subdomainfinder/__init__.py
--rw-------   0 u0_a189  (10189) u0_a189  (10189)       83 2023-04-19 18:46:46.000000 subdomainfinder-1.0/subdomainfinder/__main__.py
-drwx------   0 u0_a189  (10189) u0_a189  (10189)        0 2023-04-19 19:44:21.105066 subdomainfinder-1.0/subdomainfinder.egg-info/
--rw-------   0 u0_a189  (10189) u0_a189  (10189)     1792 2023-04-19 19:44:20.000000 subdomainfinder-1.0/subdomainfinder.egg-info/PKG-INFO
--rw-------   0 u0_a189  (10189) u0_a189  (10189)      310 2023-04-19 19:44:21.000000 subdomainfinder-1.0/subdomainfinder.egg-info/SOURCES.txt
--rw-------   0 u0_a189  (10189) u0_a189  (10189)        1 2023-04-19 19:44:20.000000 subdomainfinder-1.0/subdomainfinder.egg-info/dependency_links.txt
--rw-------   0 u0_a189  (10189) u0_a189  (10189)       67 2023-04-19 19:44:20.000000 subdomainfinder-1.0/subdomainfinder.egg-info/entry_points.txt
--rw-------   0 u0_a189  (10189) u0_a189  (10189)       14 2023-04-19 19:44:20.000000 subdomainfinder-1.0/subdomainfinder.egg-info/requires.txt
--rw-------   0 u0_a189  (10189) u0_a189  (10189)       26 2023-04-19 19:44:20.000000 subdomainfinder-1.0/subdomainfinder.egg-info/top_level.txt
+drwx------   0 u0_a189  (10189) u0_a189  (10189)        0 2023-04-19 20:10:26.751889 subdomainfinder-1.1/
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)     1792 2023-04-19 20:10:26.751889 subdomainfinder-1.1/PKG-INFO
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)      984 2023-04-19 19:02:43.000000 subdomainfinder-1.1/README.md
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)       38 2023-04-19 20:10:26.751889 subdomainfinder-1.1/setup.cfg
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)     1217 2023-04-19 20:10:09.000000 subdomainfinder-1.1/setup.py
+drwx------   0 u0_a189  (10189) u0_a189  (10189)        0 2023-04-19 20:10:26.748556 subdomainfinder-1.1/subdomainfinder/
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)     6137 2023-04-19 20:07:30.000000 subdomainfinder-1.1/subdomainfinder/__init__.py
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)       89 2023-04-19 20:09:04.000000 subdomainfinder-1.1/subdomainfinder/__main__.py
+drwx------   0 u0_a189  (10189) u0_a189  (10189)        0 2023-04-19 20:10:26.751889 subdomainfinder-1.1/subdomainfinder.egg-info/
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)     1792 2023-04-19 20:10:26.000000 subdomainfinder-1.1/subdomainfinder.egg-info/PKG-INFO
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)      310 2023-04-19 20:10:26.000000 subdomainfinder-1.1/subdomainfinder.egg-info/SOURCES.txt
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)        1 2023-04-19 20:10:26.000000 subdomainfinder-1.1/subdomainfinder.egg-info/dependency_links.txt
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)       67 2023-04-19 20:10:26.000000 subdomainfinder-1.1/subdomainfinder.egg-info/entry_points.txt
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)       14 2023-04-19 20:10:26.000000 subdomainfinder-1.1/subdomainfinder.egg-info/requires.txt
+-rw-------   0 u0_a189  (10189) u0_a189  (10189)       26 2023-04-19 20:10:26.000000 subdomainfinder-1.1/subdomainfinder.egg-info/top_level.txt
```

### Comparing `subdomainfinder-1.0/PKG-INFO` & `subdomainfinder-1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subdomainfinder
-Version: 1.0
+Version: 1.1
 Summary: A python based tool for finding subdomains of a domain.
 Home-page: https://github.com/ankushbhagatofficial/subdomain-finder
 Author: Ankush Bhagat
 Author-email: <ankushbhagatofficial@gmail.com>
 License: UNKNOWN
 Description: 
         <h1 align="center">subdomainfinder</h1>
```

### Comparing `subdomainfinder-1.0/README.md` & `subdomainfinder-1.1/README.md`

 * *Files identical despite different names*

### Comparing `subdomainfinder-1.0/setup.py` & `subdomainfinder-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "PYPIREADME.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0'
+VERSION = '1.1'
 DESCRIPTION = 'A python based tool for finding subdomains of a domain.'
 
 # Setting up
 setup(
     name='subdomainfinder',
     version=VERSION,
     author='Ankush Bhagat',
```

### Comparing `subdomainfinder-1.0/subdomainfinder/__init__.py` & `subdomainfinder-1.1/subdomainfinder/__init__.py`

 * *Files identical despite different names*

### Comparing `subdomainfinder-1.0/subdomainfinder.egg-info/PKG-INFO` & `subdomainfinder-1.1/subdomainfinder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: subdomainfinder
-Version: 1.0
+Version: 1.1
 Summary: A python based tool for finding subdomains of a domain.
 Home-page: https://github.com/ankushbhagatofficial/subdomain-finder
 Author: Ankush Bhagat
 Author-email: <ankushbhagatofficial@gmail.com>
 License: UNKNOWN
 Description: 
         <h1 align="center">subdomainfinder</h1>
```


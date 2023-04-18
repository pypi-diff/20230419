# Comparing `tmp/icecube-skywriter-0.0.1.tar.gz` & `tmp/icecube-skywriter-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icecube-skywriter-0.0.1.tar", last modified: Tue Apr 18 22:27:40 2023, max compression
+gzip compressed data, was "icecube-skywriter-0.0.2.tar", last modified: Tue Apr 18 22:32:32 2023, max compression
```

## Comparing `icecube-skywriter-0.0.1.tar` & `icecube-skywriter-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:27:40.369558 icecube-skywriter-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1085 2023-04-18 22:27:37.000000 icecube-skywriter-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1930 2023-04-18 22:27:40.369558 icecube-skywriter-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1013 2023-04-18 22:27:37.000000 icecube-skywriter-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:27:40.365558 icecube-skywriter-0.0.1/icecube_skywriter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1930 2023-04-18 22:27:40.000000 icecube-skywriter-0.0.1/icecube_skywriter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      305 2023-04-18 22:27:40.000000 icecube-skywriter-0.0.1/icecube_skywriter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 22:27:40.000000 icecube-skywriter-0.0.1/icecube_skywriter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-04-18 22:27:40.000000 icecube-skywriter-0.0.1/icecube_skywriter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 22:27:40.000000 icecube-skywriter-0.0.1/icecube_skywriter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-04-18 22:27:40.369558 icecube-skywriter-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       76 2023-04-18 22:27:37.000000 icecube-skywriter-0.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:27:40.369558 icecube-skywriter-0.0.1/skywriter/
--rw-r--r--   0 root         (0) root         (0)      592 2023-04-18 22:27:38.000000 icecube-skywriter-0.0.1/skywriter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8376 2023-04-18 22:27:37.000000 icecube-skywriter-0.0.1/skywriter/i3_to_json.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 22:27:37.000000 icecube-skywriter-0.0.1/skywriter/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:32:32.746662 icecube-skywriter-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1085 2023-04-18 22:32:30.000000 icecube-skywriter-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-04-18 22:32:32.746662 icecube-skywriter-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1013 2023-04-18 22:32:30.000000 icecube-skywriter-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:32:32.746662 icecube-skywriter-0.0.2/icecube_skywriter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1926 2023-04-18 22:32:32.000000 icecube-skywriter-0.0.2/icecube_skywriter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      305 2023-04-18 22:32:32.000000 icecube-skywriter-0.0.2/icecube_skywriter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 22:32:32.000000 icecube-skywriter-0.0.2/icecube_skywriter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-04-18 22:32:32.000000 icecube-skywriter-0.0.2/icecube_skywriter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-04-18 22:32:32.000000 icecube-skywriter-0.0.2/icecube_skywriter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1655 2023-04-18 22:32:32.746662 icecube-skywriter-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       76 2023-04-18 22:32:30.000000 icecube-skywriter-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 22:32:32.746662 icecube-skywriter-0.0.2/skywriter/
+-rw-r--r--   0 root         (0) root         (0)      592 2023-04-18 22:32:30.000000 icecube-skywriter-0.0.2/skywriter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8376 2023-04-18 22:32:30.000000 icecube-skywriter-0.0.2/skywriter/i3_to_json.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-18 22:32:30.000000 icecube-skywriter-0.0.2/skywriter/py.typed
```

### Comparing `icecube-skywriter-0.0.1/LICENSE` & `icecube-skywriter-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `icecube-skywriter-0.0.1/PKG-INFO` & `icecube-skywriter-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: icecube-skywriter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Upstream Tools for SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skywriter
 Download-URL: https://pypi.org/project/icecube-skywriter/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skywriter/issues
 Project-URL: Source, https://github.com/icecube/skywriter
 Keywords: skymap scanner,skymap,HEALPix,neutrino,reconstruction,IceCube
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `icecube-skywriter-0.0.1/README.md` & `icecube-skywriter-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `icecube-skywriter-0.0.1/icecube_skywriter.egg-info/PKG-INFO` & `icecube-skywriter-0.0.2/icecube_skywriter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: icecube-skywriter
-Version: 0.0.1
+Version: 0.0.2
 Summary: Upstream Tools for SkyDriver & the Skymap Scanner
 Home-page: https://github.com/icecube/skywriter
 Download-URL: https://pypi.org/project/icecube-skywriter/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/icecube/skywriter/issues
 Project-URL: Source, https://github.com/icecube/skywriter
 Keywords: skymap scanner,skymap,HEALPix,neutrino,reconstruction,IceCube
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `icecube-skywriter-0.0.1/setup.cfg` & `icecube-skywriter-0.0.2/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 	skymap
 	HEALPix
 	neutrino
 	reconstruction
 	IceCube
 license = MIT
 classifiers = 
-	Development Status :: 2 - Pre-Alpha
+	Development Status :: 3 - Alpha
 	License :: OSI Approved :: MIT License
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 download_url = https://pypi.org/project/icecube-skywriter/
 project_urls =
```

### Comparing `icecube-skywriter-0.0.1/skywriter/__init__.py` & `icecube-skywriter-0.0.2/skywriter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `icecube-skywriter-0.0.1/skywriter/i3_to_json.py` & `icecube-skywriter-0.0.2/skywriter/i3_to_json.py`

 * *Files identical despite different names*


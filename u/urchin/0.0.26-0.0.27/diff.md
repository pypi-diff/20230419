# Comparing `tmp/urchin-0.0.26.tar.gz` & `tmp/urchin-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urchin-0.0.26.tar", last modified: Thu Mar  2 01:15:53 2023, max compression
+gzip compressed data, was "urchin-0.0.27.tar", last modified: Wed Apr 19 16:59:06 2023, max compression
```

## Comparing `urchin-0.0.26.tar` & `urchin-0.0.27.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-03-02 01:15:53.870700 urchin-0.0.26/
--rw-rw-r--   0 fishy     (1000) fishy     (1000)     1083 2023-02-06 18:52:25.000000 urchin-0.0.26/LICENSE
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      816 2023-03-02 01:15:53.870700 urchin-0.0.26/PKG-INFO
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      612 2023-02-06 18:52:25.000000 urchin-0.0.26/README.md
--rw-rw-r--   0 fishy     (1000) fishy     (1000)       38 2023-03-02 01:15:53.870700 urchin-0.0.26/setup.cfg
--rw-rw-r--   0 fishy     (1000) fishy     (1000)     1850 2023-03-02 01:14:19.000000 urchin-0.0.26/setup.py
-drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-03-02 01:15:53.870700 urchin-0.0.26/urchin/
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      957 2023-02-06 18:52:25.000000 urchin-0.0.26/urchin/__init__.py
--rw-rw-r--   0 fishy     (1000) fishy     (1000)   131594 2023-02-06 18:52:25.000000 urchin-0.0.26/urchin/urdf.py
--rw-rw-r--   0 fishy     (1000) fishy     (1000)   131594 2023-02-06 18:52:50.000000 urchin-0.0.26/urchin/urdf_math.py
--rw-rw-r--   0 fishy     (1000) fishy     (1000)     8010 2023-02-06 18:52:25.000000 urchin-0.0.26/urchin/utils.py
--rw-rw-r--   0 fishy     (1000) fishy     (1000)       23 2023-02-06 18:52:25.000000 urchin-0.0.26/urchin/version.py
-drwxrwxr-x   0 fishy     (1000) fishy     (1000)        0 2023-03-02 01:15:53.870700 urchin-0.0.26/urchin.egg-info/
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      816 2023-03-02 01:15:53.000000 urchin-0.0.26/urchin.egg-info/PKG-INFO
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      263 2023-03-02 01:15:53.000000 urchin-0.0.26/urchin.egg-info/SOURCES.txt
--rw-rw-r--   0 fishy     (1000) fishy     (1000)        1 2023-03-02 01:15:53.000000 urchin-0.0.26/urchin.egg-info/dependency_links.txt
--rw-rw-r--   0 fishy     (1000) fishy     (1000)      174 2023-03-02 01:15:53.000000 urchin-0.0.26/urchin.egg-info/requires.txt
--rw-rw-r--   0 fishy     (1000) fishy     (1000)        7 2023-03-02 01:15:53.000000 urchin-0.0.26/urchin.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:59:06.469039 urchin-0.0.27/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-04-19 16:58:34.000000 urchin-0.0.27/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-19 16:59:06.469039 urchin-0.0.27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-04-19 16:58:34.000000 urchin-0.0.27/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 16:59:06.469039 urchin-0.0.27/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-04-19 16:58:34.000000 urchin-0.0.27/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:59:06.469039 urchin-0.0.27/urchin/
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-04-19 16:58:34.000000 urchin-0.0.27/urchin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131594 2023-04-19 16:58:34.000000 urchin-0.0.27/urchin/urdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8010 2023-04-19 16:58:34.000000 urchin-0.0.27/urchin/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 16:58:34.000000 urchin-0.0.27/urchin/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 16:59:06.469039 urchin-0.0.27/urchin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-19 16:59:06.000000 urchin-0.0.27/urchin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-19 16:59:06.000000 urchin-0.0.27/urchin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 16:59:06.000000 urchin-0.0.27/urchin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-19 16:59:06.000000 urchin-0.0.27/urchin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 16:59:06.000000 urchin-0.0.27/urchin.egg-info/top_level.txt
```

### Comparing `urchin-0.0.26/LICENSE` & `urchin-0.0.27/LICENSE`

 * *Files identical despite different names*

### Comparing `urchin-0.0.26/PKG-INFO` & `urchin-0.0.27/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urchin
-Version: 0.0.26
+Version: 0.0.27
 Summary: URDF parser and manipulator for Python
 Home-page: https://github.com/fishbotics/urchin
 Author: Adam Fishman
 Author-email: hello@fishbotics.com
 License: MIT License
 Keywords: robotics ros urdf robots parser
 Classifier: Development Status :: 4 - Beta
```

### Comparing `urchin-0.0.26/README.md` & `urchin-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `urchin-0.0.26/setup.py` & `urchin-0.0.27/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 requirements = [
     "lxml",  # For XML DOM Tree
     "networkx",  # For joint graph
     "numpy",  # Numpy
     "pillow",  # For texture image loading
-    "pycollada==0.6",  # COLLADA (.dae) mesh loading via trimesh
+    "pycollada>=0.6",  # COLLADA (.dae) mesh loading via trimesh
     "pyribbit>=0.1.46",  # For visualization
     "scipy",  # For trimesh, annoyingly
     "six",  # Python 2/3 compatability
     "trimesh",  # Mesh geometry loading/creation/saving
 ]
 
 dev_requirements = [
@@ -27,15 +27,15 @@
     "sphinx",  # General doc library
     "sphinx_rtd_theme",  # RTD theme for sphinx
     "sphinx-automodapi",  # For generating nice tables
 ]
 
 setup(
     name="urchin",
-    version="0.0.26",
+    version="0.0.27",
     description="URDF parser and manipulator for Python",
     long_description="URDF parser and manipulator for Python. This package is a fork of urdfpy, which seems to be no longer maintained. ",
     author="Adam Fishman",
     author_email="hello@fishbotics.com",
     license="MIT License",
     url="https://github.com/fishbotics/urchin",
     keywords="robotics ros urdf robots parser",
```

### Comparing `urchin-0.0.26/urchin/__init__.py` & `urchin-0.0.27/urchin/__init__.py`

 * *Files identical despite different names*

### Comparing `urchin-0.0.26/urchin/urdf.py` & `urchin-0.0.27/urchin/urdf.py`

 * *Files identical despite different names*

### Comparing `urchin-0.0.26/urchin/utils.py` & `urchin-0.0.27/urchin/utils.py`

 * *Files identical despite different names*

### Comparing `urchin-0.0.26/urchin.egg-info/PKG-INFO` & `urchin-0.0.27/urchin.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urchin
-Version: 0.0.26
+Version: 0.0.27
 Summary: URDF parser and manipulator for Python
 Home-page: https://github.com/fishbotics/urchin
 Author: Adam Fishman
 Author-email: hello@fishbotics.com
 License: MIT License
 Keywords: robotics ros urdf robots parser
 Classifier: Development Status :: 4 - Beta
```


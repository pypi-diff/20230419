# Comparing `tmp/mdiicons-0.0.1.tar.gz` & `tmp/mdiicons-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdiicons-0.0.1.tar", last modified: Wed Apr 19 18:48:19 2023, max compression
+gzip compressed data, was "mdiicons-0.0.2.tar", last modified: Wed Apr 19 19:01:04 2023, max compression
```

## Comparing `mdiicons-0.0.1.tar` & `mdiicons-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:48:19.212886 mdiicons-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 18:48:19.212886 mdiicons-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-19 18:48:07.000000 mdiicons-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:48:19.208886 mdiicons-0.0.1/mdiicons/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-19 18:48:07.000000 mdiicons-0.0.1/mdiicons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4288194 2023-04-19 18:48:07.000000 mdiicons-0.0.1/mdiicons/mdiicons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:48:19.212886 mdiicons-0.0.1/mdiicons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-04-19 18:48:19.000000 mdiicons-0.0.1/mdiicons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-19 18:48:19.000000 mdiicons-0.0.1/mdiicons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:48:19.000000 mdiicons-0.0.1/mdiicons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 18:48:19.000000 mdiicons-0.0.1/mdiicons.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:48:19.212886 mdiicons-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-19 18:48:07.000000 mdiicons-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:01:04.374736 mdiicons-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-19 19:01:04.374736 mdiicons-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-19 19:00:49.000000 mdiicons-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:01:04.370736 mdiicons-0.0.2/mdiicons/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-19 19:00:49.000000 mdiicons-0.0.2/mdiicons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4288194 2023-04-19 19:00:49.000000 mdiicons-0.0.2/mdiicons/mdiicons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:01:04.374736 mdiicons-0.0.2/mdiicons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-04-19 19:01:04.000000 mdiicons-0.0.2/mdiicons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-19 19:01:04.000000 mdiicons-0.0.2/mdiicons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:01:04.000000 mdiicons-0.0.2/mdiicons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 19:01:04.000000 mdiicons-0.0.2/mdiicons.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:01:04.374736 mdiicons-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-19 19:00:49.000000 mdiicons-0.0.2/setup.py
```

### Comparing `mdiicons-0.0.1/PKG-INFO` & `mdiicons-0.0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: mdiicons
-Version: 0.0.1
+Version: 0.0.2
 Summary: Material Design SVG strings for Python
+Home-page: https://github.com/Patrick762/mdiicons
 Author: Patrick762
 Author-email: <pip-mdi-icons@hosting-rt.de>
 Keywords: python,mdi,materialdesign,material design,materialdesignicons,material design icons,icons
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
+[![PyPI version](https://badge.fury.io/py/mdiicons.svg)](https://badge.fury.io/py/mdiicons)
+
 # mdi-py
 Material Design SVG strings for Python
 
 This library uses the mdi font from [Pictogrammers.com](https://pictogrammers.com/docs/library/mdi/getting-started/webfont/) to generate a python compatible dict.
 
 ## Examples
```

### Comparing `mdiicons-0.0.1/mdiicons/mdiicons.py` & `mdiicons-0.0.2/mdiicons/mdiicons.py`

 * *Files identical despite different names*

### Comparing `mdiicons-0.0.1/mdiicons.egg-info/PKG-INFO` & `mdiicons-0.0.2/mdiicons.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: mdiicons
-Version: 0.0.1
+Version: 0.0.2
 Summary: Material Design SVG strings for Python
+Home-page: https://github.com/Patrick762/mdiicons
 Author: Patrick762
 Author-email: <pip-mdi-icons@hosting-rt.de>
 Keywords: python,mdi,materialdesign,material design,materialdesignicons,material design icons,icons
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 
 
+[![PyPI version](https://badge.fury.io/py/mdiicons.svg)](https://badge.fury.io/py/mdiicons)
+
 # mdi-py
 Material Design SVG strings for Python
 
 This library uses the mdi font from [Pictogrammers.com](https://pictogrammers.com/docs/library/mdi/getting-started/webfont/) to generate a python compatible dict.
 
 ## Examples
```

### Comparing `mdiicons-0.0.1/setup.py` & `mdiicons-0.0.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Material Design SVG strings for Python'
 
 # Setting up
 setup(
     name="mdiicons",
     version=VERSION,
     author="Patrick762",
     author_email="<pip-mdi-icons@hosting-rt.de>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
+    url="https://github.com/Patrick762/mdiicons",
     packages=find_packages(),
     install_requires=[],
     keywords=['python', 'mdi', 'materialdesign', 'material design', 'materialdesignicons', 'material design icons', 'icons'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
```


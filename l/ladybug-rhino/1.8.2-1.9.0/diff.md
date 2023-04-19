# Comparing `tmp/ladybug-rhino-1.8.2.tar.gz` & `tmp/ladybug-rhino-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ladybug-rhino-1.8.2.tar", last modified: Thu May 14 19:23:05 2020, max compression
+gzip compressed data, was "dist/ladybug-rhino-1.9.0.tar", last modified: Thu Jun  4 20:15:33 2020, max compression
```

## Comparing `ladybug-rhino-1.8.2.tar` & `ladybug-rhino-1.9.0.tar`

### file list

```diff
@@ -1,52 +1,54 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/docs/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/docs/_templates/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3668 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/docs/_templates/layout.html
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/docs/_build/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/docs/_build/docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/docs/_build/docs/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/docs/_build/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/docs/_build/.nojekyll
--rw-rw-r--   0 travis    (2000) travis    (2000)      373 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/docs/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)     7224 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/docs/conf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/docs/index.rst
--rw-rw-r--   0 travis    (2000) travis    (2000)       80 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/docs/modules.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/docs/_static/
--rw-rw-r--   0 travis    (2000) travis    (2000)      899 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/docs/_static/custom.css
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/CODE_OF_CONDUCT.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2179 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/ladybug_rhino.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2179 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/ladybug_rhino.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/ladybug_rhino.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/ladybug_rhino.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      943 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/ladybug_rhino.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       25 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/ladybug_rhino.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/.releaserc.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     1154 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/pass_tests.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      144 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/CONTRIBUTING.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1118 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/LICENSE
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/ladybug_rhino/
--rw-rw-r--   0 travis    (2000) travis    (2000)     8448 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/togeometry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5817 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/text.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4223 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/viewport.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6220 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/planarize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5603 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/fromobjects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/bakeobjects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2848 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7091 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/fromgeometry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       47 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3495 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/bakegeometry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2251 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/colorize.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9412 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/intersect.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1874 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/baketext.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5845 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/ladybug_rhino/grasshopper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/dev-requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1027 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/deploy.sh
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-05-14 19:23:05.000000 ladybug-rhino-1.8.2/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)      327 2020-05-14 19:22:17.000000 ladybug-rhino-1.8.2/tests/togeometry_test.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/docs/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/docs/_templates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3668 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/docs/_templates/layout.html
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/docs/_build/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/docs/_build/docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/docs/_build/docs/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       16 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/docs/_build/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/docs/_build/.nojekyll
+-rw-rw-r--   0 travis    (2000) travis    (2000)      373 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/docs/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7182 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/docs/conf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      250 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/docs/index.rst
+-rw-rw-r--   0 travis    (2000) travis    (2000)       80 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/docs/modules.rst
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/docs/_static/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      899 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/docs/_static/custom.css
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2277 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/PKG-INFO
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/ladybug_rhino.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2277 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/ladybug_rhino.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/ladybug_rhino.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       14 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/ladybug_rhino.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      992 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/ladybug_rhino.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/ladybug_rhino.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/.releaserc.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1244 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)       40 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/pass_tests.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      144 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/CONTRIBUTING.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1118 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/LICENSE
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/ladybug_rhino/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8453 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/togeometry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6073 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/text.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      818 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/color.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4177 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/viewport.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6204 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/planarize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5708 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/fromobjects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2024 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/bakeobjects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2848 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6924 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/fromgeometry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2190 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/download.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3464 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/bakegeometry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2127 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/colorize.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9412 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/intersect.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1874 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/baketext.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5854 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/ladybug_rhino/grasshopper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/dev-requirements.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1027 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/setup.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/deploy.sh
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-04 20:15:33.000000 ladybug-rhino-1.9.0/tests/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      327 2020-06-04 20:14:44.000000 ladybug-rhino-1.9.0/tests/togeometry_test.py
```

### Comparing `ladybug-rhino-1.8.2/docs/_templates/layout.html` & `ladybug-rhino-1.9.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ladybug-rhino-1.8.2/docs/conf.py` & `ladybug-rhino-1.9.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,16 +222,15 @@
 # -- Options for autodoc extension --------------------------------------------
 autodoc_default_options = {
     'inherited-members': True,
 }
 
 autodoc_member_order = 'groupwise'
 
-autodoc_mock_imports = ["Rhino", "Grasshopper", "ladybug_dotnet",
-                        "scriptcontext", "System"]
+autodoc_mock_imports = ["Rhino", "Grasshopper", "scriptcontext", "System"]
 
 def setup(app):
     """Run custom code with access to the Sphinx application object
     Args:
         app: the Sphinx application object
     """
```

### Comparing `ladybug-rhino-1.8.2/docs/_static/custom.css` & `ladybug-rhino-1.9.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ladybug-rhino-1.8.2/PKG-INFO` & `ladybug-rhino-1.9.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 Metadata-Version: 2.1
 Name: ladybug-rhino
-Version: 1.8.2
+Version: 1.9.0
 Summary: A library for communicating between Ladybug Tools core libraries and Rhinoceros CAD.
 Home-page: https://github.com/ladybug-tools/ladybug-rhino
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/ladybug-tools/ladybug-rhino.svg?branch=master)](https://travis-ci.org/ladybug-tools/ladybug-rhino)
         
         [![IronPython](https://img.shields.io/badge/ironpython-2.7-red.svg)](https://github.com/IronLanguages/ironpython2/releases/tag/ipy-2.7.8/)
         
-        
         # ladybug-rhino
+        
         A library for communicating between Ladybug Tools core libraries and Rhinoceros CAD.
         
-        This library is used by both the Grasshopper and Rhino plugins to communicate with the
-        ladybug and honeybee cores.
+        This library is used by both the Grasshopper and Rhino plugins to communicate with
+        the ladybug core Python library. Note that this library has dependencies
+        on Rhino SDK and Grasshopper SDK. It is NOT intended to be run with cPython.
         
         ## Installation
-        ```
-        pip install ladybug-rhino
-        ```
         
-        ## QuickStart
         ```python
-        import ladybug_rhino
-        
+        pip install ladybug-rhino
         ```
         
         ## [API Documentation](http://ladybug-tools.github.io/ladybug-rhino/docs/)
         
         ## Local Development
+        
         1. Clone this repo locally
-        ```
+        
+        ```python
         git clone git@github.com:ladybug-tools/ladybug-rhino
         
         # or
         
         git clone https://github.com/ladybug-tools/ladybug-rhino
         ```
-        2. Install dependencies:
-        ```
+        
+        2. Install dependencies
+        
+        ```console
         cd ladybug-rhino
         pip install -r dev-requirements.txt
         pip install -r requirements.txt
         pip install pythonnet
         pip install rhinoinside
         ```
         
-        3. Generate Documentation:
+        3. Generate Documentation
+        
         ```console
         sphinx-apidoc -f -e -d 4 -o ./docs ./ladybug_rhino
         sphinx-build -b html ./docs ./docs/_build/docs
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino.egg-info/PKG-INFO` & `ladybug-rhino-1.9.0/ladybug_rhino.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,58 +1,59 @@
 Metadata-Version: 2.1
 Name: ladybug-rhino
-Version: 1.8.2
+Version: 1.9.0
 Summary: A library for communicating between Ladybug Tools core libraries and Rhinoceros CAD.
 Home-page: https://github.com/ladybug-tools/ladybug-rhino
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/ladybug-tools/ladybug-rhino.svg?branch=master)](https://travis-ci.org/ladybug-tools/ladybug-rhino)
         
         [![IronPython](https://img.shields.io/badge/ironpython-2.7-red.svg)](https://github.com/IronLanguages/ironpython2/releases/tag/ipy-2.7.8/)
         
-        
         # ladybug-rhino
+        
         A library for communicating between Ladybug Tools core libraries and Rhinoceros CAD.
         
-        This library is used by both the Grasshopper and Rhino plugins to communicate with the
-        ladybug and honeybee cores.
+        This library is used by both the Grasshopper and Rhino plugins to communicate with
+        the ladybug core Python library. Note that this library has dependencies
+        on Rhino SDK and Grasshopper SDK. It is NOT intended to be run with cPython.
         
         ## Installation
-        ```
-        pip install ladybug-rhino
-        ```
         
-        ## QuickStart
         ```python
-        import ladybug_rhino
-        
+        pip install ladybug-rhino
         ```
         
         ## [API Documentation](http://ladybug-tools.github.io/ladybug-rhino/docs/)
         
         ## Local Development
+        
         1. Clone this repo locally
-        ```
+        
+        ```python
         git clone git@github.com:ladybug-tools/ladybug-rhino
         
         # or
         
         git clone https://github.com/ladybug-tools/ladybug-rhino
         ```
-        2. Install dependencies:
-        ```
+        
+        2. Install dependencies
+        
+        ```console
         cd ladybug-rhino
         pip install -r dev-requirements.txt
         pip install -r requirements.txt
         pip install pythonnet
         pip install rhinoinside
         ```
         
-        3. Generate Documentation:
+        3. Generate Documentation
+        
         ```console
         sphinx-apidoc -f -e -d 4 -o ./docs ./ladybug_rhino
         sphinx-build -b html ./docs ./docs/_build/docs
         ```
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 2.7
```

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino.egg-info/SOURCES.txt` & `ladybug-rhino-1.9.0/ladybug_rhino.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -20,16 +20,18 @@
 docs/_build/docs/README.md
 docs/_static/custom.css
 docs/_templates/layout.html
 ladybug_rhino/__init__.py
 ladybug_rhino/bakegeometry.py
 ladybug_rhino/bakeobjects.py
 ladybug_rhino/baketext.py
+ladybug_rhino/color.py
 ladybug_rhino/colorize.py
 ladybug_rhino/config.py
+ladybug_rhino/download.py
 ladybug_rhino/fromgeometry.py
 ladybug_rhino/fromobjects.py
 ladybug_rhino/grasshopper.py
 ladybug_rhino/intersect.py
 ladybug_rhino/planarize.py
 ladybug_rhino/text.py
 ladybug_rhino/togeometry.py
```

### Comparing `ladybug-rhino-1.8.2/README.md` & `ladybug-rhino-1.9.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 [![Build Status](https://travis-ci.org/ladybug-tools/ladybug-rhino.svg?branch=master)](https://travis-ci.org/ladybug-tools/ladybug-rhino)
 
 [![IronPython](https://img.shields.io/badge/ironpython-2.7-red.svg)](https://github.com/IronLanguages/ironpython2/releases/tag/ipy-2.7.8/)
 
-
 # ladybug-rhino
+
 A library for communicating between Ladybug Tools core libraries and Rhinoceros CAD.
 
-This library is used by both the Grasshopper and Rhino plugins to communicate with the
-ladybug and honeybee cores.
+This library is used by both the Grasshopper and Rhino plugins to communicate with
+the ladybug core Python library. Note that this library has dependencies
+on Rhino SDK and Grasshopper SDK. It is NOT intended to be run with cPython.
 
 ## Installation
-```
-pip install ladybug-rhino
-```
 
-## QuickStart
 ```python
-import ladybug_rhino
-
+pip install ladybug-rhino
 ```
 
 ## [API Documentation](http://ladybug-tools.github.io/ladybug-rhino/docs/)
 
 ## Local Development
+
 1. Clone this repo locally
-```
+
+```python
 git clone git@github.com:ladybug-tools/ladybug-rhino
 
 # or
 
 git clone https://github.com/ladybug-tools/ladybug-rhino
 ```
-2. Install dependencies:
-```
+
+2. Install dependencies
+
+```console
 cd ladybug-rhino
 pip install -r dev-requirements.txt
 pip install -r requirements.txt
 pip install pythonnet
 pip install rhinoinside
 ```
 
-3. Generate Documentation:
+3. Generate Documentation
+
 ```console
 sphinx-apidoc -f -e -d 4 -o ./docs ./ladybug_rhino
 sphinx-build -b html ./docs ./docs/_build/docs
 ```
```

### Comparing `ladybug-rhino-1.8.2/.travis.yml` & `ladybug-rhino-1.9.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `ladybug-rhino-1.8.2/LICENSE` & `ladybug-rhino-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino/togeometry.py` & `ladybug-rhino-1.9.0/ladybug_rhino/togeometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,28 +114,28 @@
         for face in geo.Faces:
             if face.IsQuad:
                 all_verts = (pts[face[0]], pts[face[1]], pts[face[2]], pts[face[3]])
             else:
                 all_verts = (pts[face[0]], pts[face[1]], pts[face[2]])
             faces.append(Face3D(all_verts))
     else:  # convert each Brep Face to a Face3D
-        meshing_parameters = meshing_parameters or rg.MeshingParameters.Default # default
+        meshing_parameters = meshing_parameters or rg.MeshingParameters.Default  # default
         for b_face in geo.Faces:
             if b_face.IsPlanar(tolerance):
                 all_verts = []
                 for count in range(b_face.Loops.Count):  # Each loop is a boundary/hole
                     success, loop_pline = \
                         b_face.Loops.Item[count].To3dCurve().TryGetPolyline()
                     if not success:  # Failed to get a polyline; there's a curved edge
                         loop_verts = _planar.planar_face_curved_edge_vertices(
                             b_face, count, meshing_parameters)
                         all_verts.append(loop_verts)
                     else:  # we have a polyline representing the loop
                         all_verts.append([to_point3d(loop_pline.Item[i])
-                                        for i in range(loop_pline.Count - 1)])
+                                          for i in range(loop_pline.Count - 1)])
                 if len(all_verts) == 1:  # No holes in the shape
                     faces.append(Face3D(all_verts[0]))
                 else:  # There's at least one hole in the shape
                     faces.append(
                         Face3D(boundary=all_verts[0], holes=all_verts[1:]))
             else:  # curved face must be meshed into planar Face3D objects
                 faces.extend(_planar.curved_surface_faces(b_face, meshing_parameters))
@@ -148,17 +148,18 @@
     Args:
         geo: A Rhino Brep, Surface ro Mesh that will be converted into a single
             Ladybug Polyface3D.
         meshing_parameters: Optional Rhino Meshing Parameters to describe how
             curved faces should be converted into planar elements. If None,
             Rhino's Default Meshing Parameters will be used.
     """
-    mesh_par = meshing_parameters or rg.MeshingParameters.Default # default
+    mesh_par = meshing_parameters or rg.MeshingParameters.Default  # default
     return Polyface3D.from_faces(to_face3d(geo, mesh_par), tolerance)
 
+
 def to_mesh3d(mesh, color_by_face=True):
     """Ladybug Mesh3D from Rhino Mesh."""
     lb_verts = tuple(to_point3d(pt) for pt in mesh.Vertices)
     lb_faces, colors = _extract_mesh_faces_colors(mesh, color_by_face)
     return Mesh3D(lb_verts, lb_faces, colors)
```

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino/text.py` & `ladybug-rhino-1.9.0/ladybug_rhino/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,24 @@
 """Functions to add text to the Rhino scene and create Grasshopper text objects."""
+import math
 
 from .fromgeometry import from_plane
+from .color import black
 
 try:
     import Rhino as rh
     import System.Guid as guid
 except ImportError as e:
     raise ImportError(
         "Failed to import Rhino.\n{}".format(e))
 try:
     import Grasshopper as gh
 except ImportError:
     print('Failed to import Grasshopper.\n'
           'Only functions for adding text to Rhino will be availabe.')
-try:
-    from ladybug_dotnet.color import black
-except ImportError as e:
-    black = None
-    print("Failed to import ladybug_dotnet.\n{}".format(e))
-
-from math import sqrt
 
 
 def text_objects(text, plane, height, font='Arial',
                  horizontal_alignment=0, vertical_alignment=5):
     """Generate a Bake-able Grasshopper text object from a text string and ladybug Plane.
 
     Args:
@@ -108,15 +103,15 @@
         point = plane.PointAt(1, 1)
 
         plane.Transform(xform)
         point.Transform(xform)
         dd = point.DistanceTo(plane.Origin)
 
         text.TextPlane = plane
-        text.Height *= dd / sqrt(2)
+        text.Height *= dd / math.sqrt(2)
         new_text = TextGoo(text)
 
         new_text.m_value.Bold = self.m_value.Bold
         new_text.m_value.Italic = self.m_value.Italic
         new_text.m_value.FontFace = self.m_value.FontFace
         return new_text
 
@@ -145,26 +140,42 @@
         id = doc.Objects.AddText(self.m_value, att)
         return True, id
 
 
 class AlignmentTypes(object):
     """Enumeration of text alignment types."""
 
-    HORIZONTAL = {0: rh.DocObjects.TextHorizontalAlignment.Left,
-                  1: rh.DocObjects.TextHorizontalAlignment.Center,
-                  2: rh.DocObjects.TextHorizontalAlignment.Right}
-
-    VERTICAL = {0: rh.DocObjects.TextVerticalAlignment.Top,
-                1: rh.DocObjects.TextVerticalAlignment.MiddleOfTop,
-                2: rh.DocObjects.TextVerticalAlignment.BottomOfTop,
-                3: rh.DocObjects.TextVerticalAlignment.Middle,
-                4: rh.DocObjects.TextVerticalAlignment.MiddleOfBottom,
-                5: rh.DocObjects.TextVerticalAlignment.Bottom,
-                6: rh.DocObjects.TextVerticalAlignment.BottomOfBoundingBox}
+    _HORIZONTAL = (rh.DocObjects.TextHorizontalAlignment.Left,
+                   rh.DocObjects.TextHorizontalAlignment.Center,
+                   rh.DocObjects.TextHorizontalAlignment.Right)
+
+    _VERTICAL = (rh.DocObjects.TextVerticalAlignment.Top,
+                 rh.DocObjects.TextVerticalAlignment.MiddleOfTop,
+                 rh.DocObjects.TextVerticalAlignment.BottomOfTop,
+                 rh.DocObjects.TextVerticalAlignment.Middle,
+                 rh.DocObjects.TextVerticalAlignment.MiddleOfBottom,
+                 rh.DocObjects.TextVerticalAlignment.Bottom,
+                 rh.DocObjects.TextVerticalAlignment.BottomOfBoundingBox)
 
     @classmethod
     def horizontal(cls, field_number):
-        return cls.HORIZONTAL[field_number]
+        """Get a Rhino horizontal alignment object by its integer field number.
+
+        * 0 - Left
+        * 1 - Center
+        * 2 - Right
+        """
+        return cls._HORIZONTAL[field_number]
 
     @classmethod
     def vertical(cls, field_number):
-        return cls.VERTICAL[field_number]
+        """Get a Rhino vertical alignment object by its integer field number.
+
+        0 - Top
+        1 - MiddleOfTop
+        2 - BottomOfTop
+        3 - Middle
+        4 - MiddleOfBottom
+        5 - Bottom
+        6 - BottomOfBoundingBox
+        """
+        return cls._VERTICAL[field_number]
```

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino/viewport.py` & `ladybug-rhino-1.9.0/ladybug_rhino/viewport.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """Functions for getting viewport properties, creating new viewports, and editing them."""
+import math
 
 try:
     import Rhino.Geometry as rg
 except ImportError as e:
     raise ImportError("Failed to import Rhino.\n{}".format(e))
 
 try:  # Try to import tolerance from the active Rhino document
     import scriptcontext as sc
-except ImportError:  # No Rhino doc is available. Use Rhino's default.
+except ImportError as e:  # No Rhino doc is available. This module is useless.
     raise ImportError("Failed to import Rhino scriptcontext.\n{}".format(e))
 
-import math
-
 
 def camera_oriented_plane(origin):
     """Get a Rhino Plane that is oriented facing the camera.
 
     Args:
         origin: A Rhino Point for the origin of the plane.
     """
@@ -29,34 +28,35 @@
     """Get a Rhino Viewport object using the name of the viewport.
 
     Args:
         view_name: Text for the name of the Rhino Viewport. If None, the
             current Rhino viewport will be used.
     """
     try:
-        return sc.doc.Views.Find(view_name, False).ActiveViewport if view_name is not None \
-            else sc.doc.Views.ActiveView.ActiveViewport
-    except:
+        return sc.doc.Views.Find(view_name, False).ActiveViewport \
+            if view_name is not None else sc.doc.Views.ActiveView.ActiveViewport
+    except Exception:
         raise ValueError('Viewport "{}" was not found in the Rhino '
                          'document.'.format(view_name))
 
 
 def viewport_vh_vv(viewport, view_type):
     """Get the horizontal angle (vh) and the vertical angle (vv) from a viewport.
-    
+
     Args:
         viewport: A Rhino ViewPort object for which properties will be extracted.
         view_type: An integer to set the view type (-vt). Choose from the
             choices below.
-                * 0 Perspective (v)
-                * 1 Hemispherical fisheye (h)
-                * 2 Parallel (l)
-                * 3 Cylindrical panorama (c)
-                * 4 Angular fisheye (a)
-                * 5 Planisphere [stereographic] projection (s)
+
+            * 0 Perspective (v)
+            * 1 Hemispherical fisheye (h)
+            * 2 Parallel (l)
+            * 3 Cylindrical panorama (c)
+            * 4 Angular fisheye (a)
+            * 5 Planisphere [stereographic] projection (s)
     """
     if view_type == 0:  # perspective
         right_vec = viewport.GetFrustumRightPlane()[1][1]
         left_vec = viewport.GetFrustumLeftPlane()[1][1]
         h_angle = 180 - math.degrees(rg.Vector3d.VectorAngle(right_vec, left_vec))
         bottom_vec = viewport.GetFrustumBottomPlane()[1][1]
         top_vec = viewport.GetFrustumTopPlane()[1][1]
@@ -76,25 +76,25 @@
 def viewport_properties(viewport, view_type=None):
     """Get a dictionary of properties of a Rhino viewport.
 
     Args:
         viewport: A Rhino ViewPort object for which properties will be extracted.
         view_type: An integer to set the view type (-vt). Choose from the
             choices below or set to None to have it derived from the viewport.
-                * 0 Perspective (v)
-                * 1 Hemispherical fisheye (h)
-                * 2 Parallel (l)
-                * 3 Cylindrical panorama (c)
-                * 4 Angular fisheye (a)
-                * 5 Planisphere [stereographic] projection (s)
+
+            * 0 Perspective (v)
+            * 1 Hemispherical fisheye (h)
+            * 2 Parallel (l)
+            * 3 Cylindrical panorama (c)
+            * 4 Angular fisheye (a)
+            * 5 Planisphere [stereographic] projection (s)
 
     Returns:
         A dictionary with the following keys: 'view_type', 'position', 'direction',
         'up_vector', 'h_angle', 'v_angle'
-        
     """
     # ensure that we have an integer for the view_type
     if view_type is None:
         view_type = 2 if viewport.IsParallelProjection else 0
 
     # get the position, direction and up vectors
     pos = viewport.CameraLocation
@@ -109,8 +109,8 @@
     return {
         'view_type': view_type,
         'position': (pos.X, pos.Y, pos.Z),
         'direction': (direct.X, direct.Y, direct.Z),
         'up_vector': (up_vec.X, up_vec.Y, up_vec.Z),
         'h_angle': h_angle,
         'v_angle': v_angle
-        }
+    }
```

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino/planarize.py` & `ladybug-rhino-1.9.0/ladybug_rhino/planarize.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     the adjoining curved surface is not an extrusion.
 
     Args:
         b_face: A brep face with the curved edge.
         count: An integer for the index of the loop to extract.
         meshing_parameters: Rhino Meshing Parameters to describe how
             curved edge should be converted into planar elements.
-    
+
     Returns:
         A list of ladybug Point3D objects representing the input planar face.
     """
     loop_pcrv = b_face.Loops.Item[count].To3dCurve()
     f_norm = b_face.NormalAt(0, 0)
     if f_norm.Z < 0:
         loop_pcrv.Reverse()
@@ -66,15 +66,15 @@
 def curved_surface_faces(b_face, meshing_parameters):
     """Extract Face3D objects from a curved brep face.
 
     Args:
         b_face: A curved brep face.
         meshing_parameters: Rhino Meshing Parameters to describe how
             curved edge should be converted into planar elements.
-    
+
     Returns:
         A list of ladybug Face3D objects that together approximate the input
         curved surface.
     """
     if b_face.OrientationIsReversed:
         b_face.Reverse(0, True)
     face_brep = b_face.DuplicateFace(True)
@@ -147,29 +147,29 @@
         A list of ladybug Face3D objects derived from the input mesh faces.
     """
     faces = []
     for m_face in mesh.Faces:
         if m_face.IsQuad:
             lb_face = Face3D(
                 tuple(_point3d(mesh.Vertices[i]) for i in
-                        (m_face.A, m_face.B, m_face.C, m_face.D)))
+                      (m_face.A, m_face.B, m_face.C, m_face.D)))
             if lb_face.check_planar(tolerance, False):
                 faces.append(lb_face)
             else:
                 lb_face_1 = Face3D(
                     tuple(_point3d(mesh.Vertices[i]) for i in
-                            (m_face.A, m_face.B, m_face.C)))
+                          (m_face.A, m_face.B, m_face.C)))
                 lb_face_2 = Face3D(
                     tuple(_point3d(mesh.Vertices[i]) for i in
-                            (m_face.C, m_face.D, m_face.A)))
+                          (m_face.C, m_face.D, m_face.A)))
                 faces.extend([lb_face_1, lb_face_2])
         else:
             lb_face = Face3D(
                 tuple(_point3d(mesh.Vertices[i]) for i in
-                        (m_face.A, m_face.B, m_face.C)))
+                      (m_face.A, m_face.B, m_face.C)))
             faces.append(lb_face)
     return faces
 
 
 def _point3d(point):
     """Ladybug Point3D from Rhino Point3d."""
     return Point3D(point.X, point.Y, point.Z)
```

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino/fromobjects.py` & `ladybug-rhino-1.9.0/ladybug_rhino/fromobjects.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,19 @@
 The methods here are intended to help translate groups of geometry that are commonly
 generated by several objects in Ladybug core (ie. legends, compasses, etc.)
 """
 
 from .fromgeometry import from_mesh3d, from_arc2d, from_linesegment2d
 from .text import text_objects
 
-from ladybug_geometry.geometry3d.pointvector import Point3D
-from ladybug_geometry.geometry3d.plane import Plane
+try:
+    from ladybug_geometry.geometry3d.pointvector import Point3D
+    from ladybug_geometry.geometry3d.plane import Plane
+except ImportError as e:
+    raise ImportError("Failed to import ladybug_geometry.\n{}".format(e))
 
 
 def legend_objects(legend):
     """Translate a Ladybug Legend object into Grasshopper geometry.
 
     Args:
         legend: A Ladybug Legend object to be converted to Rhino geometry.
@@ -49,16 +52,18 @@
         compass: A Ladybug Compass object to be converted to Rhino geometry.
         z: A number for the Z-coordinate to be used in translation. (Default: 0)
         custom_angles: An array of numbers between 0 and 360 to be used to
             generate custom angle labels around the compass.
         projection: Text for the name of the projection to use from the sky
             dome hemisphere to the 2D plane. If None, no altitude circles o
             labels will be drawn (Default: None). Choose from the following:
+
                 * Orthographic
                 * Stereographic
+
         font: Optional text for the font to be used in creating the text.
             (Default: 'Arial')
 
     Returns:
         A list of Rhino geometries in the following order.
 
         -   all_boundary_circles -- Three Circle objects for the compass boundary.
@@ -74,15 +79,15 @@
                 labels (if applicable).
 
         -   altitude_circles -- Circle objects for the altitude labels.
 
         -   altitude_text -- Bake-able text objects for the altitude labels.
 
      """
-     # set default variables based on the compass properties
+    # set default variables based on the compass properties
     maj_txt = compass.radius / 20
     min_txt = maj_txt / 2
 
     result = []  # list to hold all of the returned objects
     for circle in compass.all_boundary_circles:
         result.append(from_arc2d(circle, z))
 
@@ -100,24 +105,24 @@
                 txt, Plane(o=Point3D(pt.x, pt.y, z)), min_txt, font, 1, 3))
     else:
         for line in compass.ticks_from_angles(custom_angles):
             result.append(from_linesegment2d(line, z))
         for txt, pt in zip(custom_angles, compass.label_points_from_angles(custom_angles)):
             result.append(text_objects(
                 str(txt), Plane(o=Point3D(pt.x, pt.y, z)), maj_txt, font, 1, 3))
-    
+
     # generate the labels and tick marks for the altitudes
     if projection is not None:
         if projection.title() == 'Orthographic':
             for circle in compass.orthographic_altitude_circles:
                 result.append(from_arc2d(circle, z))
             for txt, pt in zip(compass.ALTITUDES, compass.orthographic_altitude_points):
                 result.append(text_objects(
                     str(txt), Plane(o=Point3D(pt.x, pt.y, z)), min_txt, font, 1, 0))
         elif projection.title() == 'Stereographic':
             for circle in compass.stereographic_altitude_circles:
                 result.append(from_arc2d(circle, z))
             for txt, pt in zip(compass.ALTITUDES, compass.stereographic_altitude_points):
                 result.append(text_objects(
                     str(txt), Plane(o=Point3D(pt.x, pt.y, z)), min_txt, font, 1, 0))
-    
+
     return result
```

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino/bakeobjects.py` & `ladybug-rhino-1.9.0/ladybug_rhino/bakeobjects.py`

 * *Files identical despite different names*

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino/config.py` & `ladybug-rhino-1.9.0/ladybug_rhino/config.py`

 * *Files identical despite different names*

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino/fromgeometry.py` & `ladybug-rhino-1.9.0/ladybug_rhino/fromgeometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 """Functions to translate from Ladybug geomtries to Rhino geometries."""
+from .config import tolerance
+from .color import color_to_color, gray
 
 try:
     import Rhino.Geometry as rg
 except ImportError as e:
     raise ImportError(
         "Failed to import Rhino Geometry.\n{}".format(e))
-try:
-    from ladybug_dotnet.color import color_to_color, gray
-except ImportError as e:
-    raise ImportError(
-        "Failed to import ladybug_dotnet.\n{}".format(e))
-from .config import tolerance
 
 
 """____________2D GEOMETRY TRANSLATORS____________"""
 
 
 def from_vector2d(vector):
     """Rhino Vector3d from ladybug Vector2D."""
@@ -40,16 +36,16 @@
     """Rhino Arc from ladybug Arc2D."""
     circle = rg.Circle(from_point2d(arc.c, z), arc.r)
     return rg.Arc(circle, rg.Interval(arc.a1, arc.a2))
 
 
 def from_polygon2d(polygon, z=0):
     """Rhino closed PolyLineCurve from ladybug Polygon2D."""
-    return rg.PolylineCurve([from_point2d(pt, z) for pt in polygon.vertices] +
-                            [from_point2d(polygon[0], z)])
+    return rg.PolylineCurve(
+        [from_point2d(pt, z) for pt in polygon.vertices] + [from_point2d(polygon[0], z)])
 
 
 def from_polyline2d(polyline, z=0):
     """Rhino closed PolyLineCurve from ladybug Polyline2D."""
     rhino_pts = [from_point2d(pt, z) for pt in polyline.vertices]
     if polyline.interpolated:
         return rg.Curve.CreateInterpolatedCurve(
@@ -142,16 +138,16 @@
 
 
 """________ADDITIONAL 3D GEOMETRY TRANSLATORS________"""
 
 
 def from_face3d_to_wireframe(face):
     """Rhino PolyLineCurve from ladybug Face3D."""
-    return rg.PolylineCurve([from_point3d(pt) for pt in face.boundary] +
-                            [from_point3d(face.boundary[0])])
+    return rg.PolylineCurve(
+        [from_point3d(pt) for pt in face.boundary] + [from_point3d(face.boundary[0])])
 
 
 def from_polyface3d_to_wireframe(polyface):
     """Rhino PolyLineCurve from ladybug Polyface3D."""
     return [from_face3d_to_wireframe(face) for face in polyface.faces]
```

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino/bakegeometry.py` & `ladybug-rhino-1.9.0/ladybug_rhino/bakegeometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from .fromgeometry import from_point2d, from_mesh2d, from_point3d, from_mesh3d, \
     from_face3d, from_polyface3d
 
 try:
     import Rhino.RhinoDoc as rhdoc
     import Rhino.DocObjects as docobj
-    import scriptcontext as sc
     doc = rhdoc.ActiveDoc
 except ImportError as e:
     raise ImportError(
         "Failed to import Rhino document attributes.\n{}".format(e))
 
 
 """____________ADD GEOMETRY TO THE RHINO SCENE____________"""
```

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino/colorize.py` & `ladybug-rhino-1.9.0/ladybug_rhino/colorize.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """Classes for colorized versions of various Rhino objects like points."""
+from .color import black
+
 try:
     import Rhino as rh
     import System.Guid as guid
 except ImportError as e:
     raise ImportError(
         "Failed to import Rhino.\n{}".format(e))
 try:
     import Grasshopper as gh
 except ImportError:
     print('Failed to import Grasshopper.\n'
           'Only functions for adding text to Rhino will be availabe.')
-try:
-    from ladybug_dotnet.color import black
-except ImportError as e:
-    black = None
-    print("Failed to import ladybug_dotnet.\n{}".format(e))
 
 
 class ColoredPoint(gh.Kernel.Types.GH_Point, gh.Kernel.IGH_BakeAwareData,
                    gh.Kernel.IGH_PreviewData):
     """A Point object with a set-able color property to change its color in Grasshopper.
 
     Args:
```

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino/intersect.py` & `ladybug-rhino-1.9.0/ladybug_rhino/intersect.py`

 * *Files identical despite different names*

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino/baketext.py` & `ladybug-rhino-1.9.0/ladybug_rhino/baketext.py`

 * *Files identical despite different names*

### Comparing `ladybug-rhino-1.8.2/ladybug_rhino/grasshopper.py` & `ladybug-rhino-1.9.0/ladybug_rhino/grasshopper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Functions for dealing with inputs and outputs from Grasshopper components."""
-from collections import namedtuple
+import collections
+
 try:
     from Grasshopper.Kernel import GH_RuntimeMessageLevel as Message
     from Grasshopper.Kernel.Types import GH_ObjectWrapper as Goo
     from Grasshopper import DataTree
     from Grasshopper.Kernel.Data import GH_Path as Path
 except ImportError:
     raise ImportError(
@@ -93,15 +94,15 @@
     Args:
         input: A Grasshopper DataTree.
 
     Returns:
         listData -- A list of namedtuples (path, dataList)
     """
     all_data = list(range(len(input.Paths)))
-    Pattern = namedtuple('Pattern', 'path list')
+    Pattern = collections.namedtuple('Pattern', 'path list')
 
     for i, path in enumerate(input.Paths):
         data = input.Branch(path)
         branch = Pattern(path, [])
 
         for d in data:
             if d is not None:
@@ -141,15 +142,15 @@
 
         -   all_data -- All data in DataTree as a flattened list.
 
         -   pattern -- A dictionary of patterns as namedtuple(path, index of last item
             on this path, path Count). Pattern is useful to un-flatten the list
             back to a DataTree.
     """
-    Pattern = namedtuple('Pattern', 'path index count')
+    Pattern = collections.namedtuple('Pattern', 'path index count')
     pattern = dict()
     all_data = []
     index = 0  # Global counter for all the data
     for i, path in enumerate(input.Paths):
         count = 0
         data = input.Branch(path)
```

### Comparing `ladybug-rhino-1.8.2/setup.py` & `ladybug-rhino-1.9.0/setup.py`

 * *Files identical despite different names*


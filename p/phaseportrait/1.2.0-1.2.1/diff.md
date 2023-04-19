# Comparing `tmp/phaseportrait-1.2.0.tar.gz` & `tmp/phaseportrait-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phaseportrait-1.2.0.tar", last modified: Tue Apr 11 10:18:15 2023, max compression
+gzip compressed data, was "phaseportrait-1.2.1.tar", last modified: Wed Apr 19 18:47:29 2023, max compression
```

## Comparing `phaseportrait-1.2.0.tar` & `phaseportrait-1.2.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:18:15.336444 phaseportrait-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-11 10:18:15.336444 phaseportrait-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/README_no_imgs.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:18:15.328443 phaseportrait-1.2.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:18:15.332444 phaseportrait-1.2.0/examples/api_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/examples/api_examples/phaseportrait2d_example.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:18:15.332444 phaseportrait-1.2.0/phaseportrait/
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/Cobweb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/Map1D.py
--rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/PhasePortrait2D.py
--rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/PhasePortrait3D.py
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/PhasePortraitManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/Trajectories2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/Trajectories3D.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:18:15.332444 phaseportrait-1.2.0/phaseportrait/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:18:15.332444 phaseportrait-1.2.0/phaseportrait/generators_base/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/generators_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/generators_base/generator_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:18:15.332444 phaseportrait-1.2.0/phaseportrait/maps/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/maps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/maps/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:18:15.332444 phaseportrait-1.2.0/phaseportrait/nullclines/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/nullclines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/nullclines/nullclines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:18:15.332444 phaseportrait-1.2.0/phaseportrait/sliders/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/sliders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/sliders/sliders.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:18:15.336444 phaseportrait-1.2.0/phaseportrait/streamlines/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/streamlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/streamlines/size_gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/streamlines/streamlines_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/streamlines/velocity_color_gradient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:18:15.336444 phaseportrait-1.2.0/phaseportrait/trajectories/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/trajectories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/trajectories/rungekutta.py
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/trajectories/trajectory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:18:15.336444 phaseportrait-1.2.0/phaseportrait/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/utils/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/phaseportrait/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 10:18:15.332444 phaseportrait-1.2.0/phaseportrait.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-11 10:18:15.000000 phaseportrait-1.2.0/phaseportrait.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-11 10:18:15.000000 phaseportrait-1.2.0/phaseportrait.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 10:18:15.000000 phaseportrait-1.2.0/phaseportrait.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 10:18:15.000000 phaseportrait-1.2.0/phaseportrait.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 10:18:15.000000 phaseportrait-1.2.0/phaseportrait.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-11 10:18:15.336444 phaseportrait-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-11 10:18:01.000000 phaseportrait-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:47:29.581390 phaseportrait-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-19 18:47:29.581390 phaseportrait-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/README_no_imgs.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:47:29.573390 phaseportrait-1.2.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:47:29.577390 phaseportrait-1.2.1/examples/api_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/examples/api_examples/phaseportrait2d_example.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:47:29.577390 phaseportrait-1.2.1/phaseportrait/
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/Cobweb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/Map1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/PhasePortrait2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/PhasePortrait3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/PhasePortraitManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3950 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/Trajectories2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/Trajectories3D.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:47:29.577390 phaseportrait-1.2.1/phaseportrait/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:47:29.577390 phaseportrait-1.2.1/phaseportrait/generators_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/generators_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/generators_base/generator_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:47:29.577390 phaseportrait-1.2.1/phaseportrait/maps/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/maps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/maps/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:47:29.577390 phaseportrait-1.2.1/phaseportrait/nullclines/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/nullclines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5078 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/nullclines/nullclines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:47:29.577390 phaseportrait-1.2.1/phaseportrait/sliders/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/sliders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/sliders/sliders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:47:29.577390 phaseportrait-1.2.1/phaseportrait/streamlines/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/streamlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/streamlines/size_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13605 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/streamlines/streamlines_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/streamlines/velocity_color_gradient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:47:29.577390 phaseportrait-1.2.1/phaseportrait/trajectories/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/trajectories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/trajectories/rungekutta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/trajectories/trajectory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:47:29.581390 phaseportrait-1.2.1/phaseportrait/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/utils/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/phaseportrait/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:47:29.577390 phaseportrait-1.2.1/phaseportrait.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-04-19 18:47:29.000000 phaseportrait-1.2.1/phaseportrait.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-19 18:47:29.000000 phaseportrait-1.2.1/phaseportrait.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:47:29.000000 phaseportrait-1.2.1/phaseportrait.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 18:47:29.000000 phaseportrait-1.2.1/phaseportrait.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 18:47:29.000000 phaseportrait-1.2.1/phaseportrait.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-19 18:47:29.581390 phaseportrait-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-19 18:47:18.000000 phaseportrait-1.2.1/setup.py
```

### Comparing `phaseportrait-1.2.0/LICENSE` & `phaseportrait-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/PKG-INFO` & `phaseportrait-1.2.1/README_no_imgs.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: phaseportrait
-Version: 1.2.0
-Summary: A python package for visualizing non-linear dynamics and chaos. (2D phase portraits, 3D chaotic trajectories, Maps, Cobweb plots...)
-Author-email: Víctor Loras <vhloras@gmail.com>, Unai Lería <unaileria@gmail.com>
-Maintainer-email: Víctor Loras <vhloras@gmail.com>, Unai Lería <unaileria@gmail.com>
-License: MIT license
-Project-URL: Documentation, https://phaseportrait.github.io/
-Project-URL: GitHub, https://github.com/phaseportrait/phaseportrait
-Project-URL: GUI, https://github.com/phaseportrait/phaseportrait-gui
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Education
-Classifier: Topic :: Scientific/Engineering
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Documentation
 
 To check out *phaseportrait*'s documentation, view some examples and read more about it, check our website or try our Graphical User Interface:
 
 
 [Documentation](https://phaseportrait.github.io/)
```

### Comparing `phaseportrait-1.2.0/phaseportrait/Cobweb.py` & `phaseportrait-1.2.1/phaseportrait/Cobweb.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/Map1D.py` & `phaseportrait-1.2.1/phaseportrait/Map1D.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/PhasePortrait2D.py` & `phaseportrait-1.2.1/phaseportrait/PhasePortrait2D.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from inspect import signature
+from typing import Literal
 
 import matplotlib.cm as mplcm
 import matplotlib.colors as mcolors
 import matplotlib.pyplot as plt
 import numpy as np
 
 from .exceptions import exceptions
@@ -225,33 +226,34 @@
         self.ax.set_yscale(self.yScale)
         self.ax.grid(grid if grid is not None else self.grid)
         
         return stream
 
 
 
-    def add_nullclines(self, *, precision=0.01, xprecision=None, yprecision=None, offset=0., density=50, xRange=None, yRange=None, dF_args=None, xcolor='r', ycolor='g', bgcolor='w', alpha=0):
+    def add_nullclines(self, *, precision=0.01, xprecision=None, yprecision=None, show: Literal['x', 'y', None]=None, offset=0., density=50, xRange=None, yRange=None, dF_args=None, xcolor='r', ycolor='g', bgcolor='w', alpha=0):
         """Adds nullclines for both axis.
 
         Args:
             precision (float, optional): Precision if not specific axis precision is specified. Defaults to 0.01.
             xprecision (float, optional): Precision for x axis nullcline. Defaults to None.
             yprecision (float, optional): Precision for y axis nullcline. Defaults to None.
+            show (Literal['x', 'y', None], optinal) : Used to show only x or y nullclines, both if None. Defaults to None.
             offset (float, optional): Specifies the value in which the countours will be drawn. Defaults to 0.
             density (int, optional): Density of grid used in interpolation. Defaults to 50.
             xRange (list[float], optional): Range of x nullcline, by default global range. Defaults to None.
             yRange (list[float], optional): Range of y nullcline, by default global range. Defaults to None.
             dF_args (dict, optional): Overrides general `dFargs` if is not None. Defaults to None.
             xcolor (str, optional): Color for x nullcline. Defaults to 'r'.
             ycolor (str, optional): Color for y nullcline. Defaults to 'g'.
             bgcolor (str, optional): Color for background. Defaults to 'w'.
             alpha (int, optional): Alpha of nullclines and background. Defaults to 0.
         """        
         self.nullclines.append(Nullcline2D(self, self.dF,
-                                          precision=precision, xprecision=xprecision, yprecision=yprecision, offset=offset, density=density, 
+                                          precision=precision, xprecision=xprecision, yprecision=yprecision, show=show, offset=offset, density=density, 
                                           xRange=xRange, yRange=yRange, dF_args=dF_args, 
                                           xcolor=xcolor, ycolor=ycolor, bgcolor=bgcolor, alpha=alpha, polar=self.Polar))
             
 
 
     def add_slider(self, param_name, *, valinit=None, valstep=0.1, valinterval=10):
         """
```

### Comparing `phaseportrait-1.2.0/phaseportrait/PhasePortrait3D.py` & `phaseportrait-1.2.1/phaseportrait/PhasePortrait3D.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/PhasePortraitManager.py` & `phaseportrait-1.2.1/phaseportrait/PhasePortraitManager.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/Trajectories2D.py` & `phaseportrait-1.2.1/phaseportrait/Trajectories2D.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/Trajectories3D.py` & `phaseportrait-1.2.1/phaseportrait/Trajectories3D.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/exceptions/exceptions.py` & `phaseportrait-1.2.1/phaseportrait/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/generators_base/generator_base.py` & `phaseportrait-1.2.1/phaseportrait/generators_base/generator_base.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/maps/map.py` & `phaseportrait-1.2.1/phaseportrait/maps/map.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/nullclines/nullclines.py` & `phaseportrait-1.2.1/phaseportrait/nullclines/nullclines.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from matplotlib.colors import to_hex
+from typing import Literal
 
 class Nullcline2D():
     """
     Nullcline2D
     --------
     Class dedicated to 2 dimensions phase portraits. 
     Useful where it is necessary to plot nulclines in a plot.
@@ -12,23 +13,24 @@
     - PhasePortrait2D 
     
     Methods
     -------
     * plot : Plots the nullclines.
     """
     
-    def __init__(self, portrait, funcion, *, precision=0.01, xprecision=None, yprecision=None, offset=0, density=50, xRange=None, yRange=None, dF_args=None, xcolor='r', ycolor='b', bgcolor='w', alpha=0, polar=False):
+    def __init__(self, portrait, funcion, *, precision=0.01, xprecision=None, yprecision=None, show: Literal['x', 'y', None]=None, offset=0, density=50, xRange=None, yRange=None, dF_args=None, xcolor='r', ycolor='b', bgcolor='w', alpha=0, polar=False):
         """Creates an instance of Nullcline2D
 
         Args:
             portrait (Object) : The class that uses Nullcline2D
             funcion (callable) : A `dF` type funcion.
             precision (float, optional) : The minimum diferencie from `offset` to be considerated a nullcline, by default 0.01
             xprecision (float, optional) : For a different precision value only in the x axis, by default `precision`
             yprecision (float, optional) : For a different precision value only in the y axis, by default `precision`
+            show (Literal['x', 'y', None], optinal) : Used to show only x or y nullclines, both if None, by default None
             offset (float, optional) : If you want, for instance, a twoclide, by default 0
             density (int, optional) : Number of inner divisions on the x axis and y axis, by default 50
             xRange (Union[float,list], optional) : The range in which the nullclines are calculated, by default `portrait.Range[0]`
             yRange (Union[float,list], optional) : The range in which the nullclines are calculated, by default `portrait.Range[1]`
             dF_args (dict, optional) : If necesary, must contain the kargs for the `dF` funcion, by default None
             xcolor (str, optional) : X nullcline color, by default 'r'
             ycolor (str, optional) : Y nullcline color], by default 'b'
@@ -37,14 +39,15 @@
             polar (bool, optional) : If the dF funcion requires polar coordinates, by default False
         """                         
         self.portrait = portrait
         self.funcion = funcion
         self.precision = precision
         self.xprecision = xprecision if xprecision is not None else precision
         self.yprecision = yprecision if yprecision is not None else precision
+        self.show = show
         self.offset = offset
         self.xcolor = to_hex(xcolor)
         self.ycolor = to_hex(ycolor)
         self.bgcolor = bgcolor
         self.density = density
         self.alpha = alpha
         self.polar = polar
@@ -87,16 +90,18 @@
                     _dr, _dt = self.funcion(_r,_t, **self.dF_args)
                     _xdF[j,i], _ydF[j,i] = _dr*np.cos(_t) - _r*np.sin(_t)*_dt, _dr*np.sin(_t) + _r*np.cos(_t)*_dt       
         else:
             for i,xx in enumerate(_x):
                 for j,yy in enumerate(_y):
                     _xdF[j,i], _ydF[j,i] = self.funcion(xx,yy, **self.dF_args)
         
-        xct = axis.contourf(_x, _y,_xdF, levels=[-self.xprecision + self.offset, self.xprecision + self.offset], colors=[self.xcolor], extend='neither')
-        yct = axis.contourf(_x, _y,_ydF, levels=[-self.yprecision + self.offset, self.yprecision + self.offset], colors=[self.ycolor], extend='neither')
-        
-        xct.cmap.set_over(self.bgcolor, alpha=self.alpha)
-        yct.cmap.set_over(self.bgcolor, alpha=self.alpha)
-        xct.cmap.set_under(self.bgcolor, alpha=self.alpha)
-        yct.cmap.set_under(self.bgcolor, alpha=self.alpha)
+        if self.show is None or self.show == 'x':
+            xct = axis.contourf(_x, _y,_xdF, levels=[-self.xprecision + self.offset, self.xprecision + self.offset], colors=[self.xcolor], extend='neither')
+            xct.cmap.set_over(self.bgcolor, alpha=self.alpha)
+            xct.cmap.set_under(self.bgcolor, alpha=self.alpha)
+
+        if self.show is None or self.show == 'y':   
+            yct = axis.contourf(_x, _y,_ydF, levels=[-self.yprecision + self.offset, self.yprecision + self.offset], colors=[self.ycolor], extend='neither')
+            yct.cmap.set_over(self.bgcolor, alpha=self.alpha)
+            yct.cmap.set_under(self.bgcolor, alpha=self.alpha)
     
         return xct, yct
```

### Comparing `phaseportrait-1.2.0/phaseportrait/sliders/sliders.py` & `phaseportrait-1.2.1/phaseportrait/sliders/sliders.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/streamlines/size_gradient.py` & `phaseportrait-1.2.1/phaseportrait/streamlines/size_gradient.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/streamlines/streamlines_base.py` & `phaseportrait-1.2.1/phaseportrait/streamlines/streamlines_base.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/streamlines/velocity_color_gradient.py` & `phaseportrait-1.2.1/phaseportrait/streamlines/velocity_color_gradient.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/trajectories/rungekutta.py` & `phaseportrait-1.2.1/phaseportrait/trajectories/rungekutta.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/trajectories/trajectory.py` & `phaseportrait-1.2.1/phaseportrait/trajectories/trajectory.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/utils/manager.py` & `phaseportrait-1.2.1/phaseportrait/utils/manager.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait/utils/utils.py` & `phaseportrait-1.2.1/phaseportrait/utils/utils.py`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/phaseportrait.egg-info/SOURCES.txt` & `phaseportrait-1.2.1/phaseportrait.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phaseportrait-1.2.0/pyproject.toml` & `phaseportrait-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 # Minimum requirements for the build system to execute.
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "phaseportrait"
-version = "1.2.0"
+version = "1.2.1"
 requires-python = ">=3.8"
 
 description = "A python package for visualizing non-linear dynamics and chaos. (2D phase portraits, 3D chaotic trajectories, Maps, Cobweb plots...)"
 
 authors = [
     {name = "Víctor Loras"  , email = "vhloras@gmail.com"}, 
     {name =  "Unai Lería"   , email =  "unaileria@gmail.com"}]
 
 maintainers = [
     {name = "Víctor Loras"  , email = "vhloras@gmail.com"}, 
     {name =  "Unai Lería"   , email =  "unaileria@gmail.com"}] 
 
 
-readme = "README_no_imgs.md"
+readme = "README.md"
 license = { text="MIT license" }
 
 classifiers = [
     "Intended Audience :: Education",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```


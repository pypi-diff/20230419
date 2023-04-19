# Comparing `tmp/polar_route-0.0.15.tar.gz` & `tmp/polar_route-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polar_route-0.0.15.tar", last modified: Thu Oct 27 15:31:37 2022, max compression
+gzip compressed data, was "polar_route-0.1.0.tar", last modified: Wed Apr 19 14:04:35 2023, max compression
```

## Comparing `polar_route-0.0.15.tar` & `polar_route-0.1.0.tar`

### file list

```diff
@@ -1,27 +1,73 @@
-drwxr-xr-x   0 jsmith     (501) staff       (20)        0 2022-10-27 15:31:37.848834 polar_route-0.0.15/
--rw-r--r--   0 jsmith     (501) staff       (20)     1081 2022-09-28 08:20:50.000000 polar_route-0.0.15/LICENSE
--rw-r--r--   0 jsmith     (501) staff       (20)       51 2022-10-24 10:18:16.000000 polar_route-0.0.15/MANIFEST.in
--rw-r--r--   0 jsmith     (501) staff       (20)     3707 2022-10-27 15:31:37.848928 polar_route-0.0.15/PKG-INFO
--rw-r--r--   0 jsmith     (501) staff       (20)     2631 2022-10-24 14:59:50.000000 polar_route-0.0.15/README.md
-drwxr-xr-x   0 jsmith     (501) staff       (20)        0 2022-10-27 15:31:37.847279 polar_route-0.0.15/polar_route/
--rw-r--r--   0 jsmith     (501) staff       (20)      346 2022-10-27 15:18:14.000000 polar_route-0.0.15/polar_route/__init__.py
--rw-r--r--   0 jsmith     (501) staff       (20)    30090 2022-10-06 08:37:44.000000 polar_route-0.0.15/polar_route/cellbox.py
--rw-r--r--   0 jsmith     (501) staff       (20)     3632 2022-10-27 13:35:29.000000 polar_route-0.0.15/polar_route/cli.py
--rw-r--r--   0 jsmith     (501) staff       (20)    46252 2022-10-27 13:35:29.000000 polar_route-0.0.15/polar_route/crossing.py
--rw-r--r--   0 jsmith     (501) staff       (20)    33398 2022-10-24 14:59:50.000000 polar_route-0.0.15/polar_route/data_loaders.py
--rw-r--r--   0 jsmith     (501) staff       (20)    38553 2022-10-17 12:11:48.000000 polar_route-0.0.15/polar_route/mesh.py
--rw-r--r--   0 jsmith     (501) staff       (20)    27107 2022-09-28 08:20:50.000000 polar_route-0.0.15/polar_route/plot.py
--rw-r--r--   0 jsmith     (501) staff       (20)    29630 2022-10-27 13:21:38.000000 polar_route-0.0.15/polar_route/route_planner.py
--rw-r--r--   0 jsmith     (501) staff       (20)     1367 2022-09-28 08:20:50.000000 polar_route-0.0.15/polar_route/transients.py
--rw-r--r--   0 jsmith     (501) staff       (20)     2429 2022-10-06 08:37:44.000000 polar_route-0.0.15/polar_route/utils.py
--rw-r--r--   0 jsmith     (501) staff       (20)    12511 2022-10-27 15:18:14.000000 polar_route-0.0.15/polar_route/vessel_performance.py
-drwxr-xr-x   0 jsmith     (501) staff       (20)        0 2022-10-27 15:31:37.848684 polar_route-0.0.15/polar_route.egg-info/
--rw-r--r--   0 jsmith     (501) staff       (20)     3707 2022-10-27 15:31:37.000000 polar_route-0.0.15/polar_route.egg-info/PKG-INFO
--rw-r--r--   0 jsmith     (501) staff       (20)      562 2022-10-27 15:31:37.000000 polar_route-0.0.15/polar_route.egg-info/SOURCES.txt
--rw-r--r--   0 jsmith     (501) staff       (20)        1 2022-10-27 15:31:37.000000 polar_route-0.0.15/polar_route.egg-info/dependency_links.txt
--rw-r--r--   0 jsmith     (501) staff       (20)      164 2022-10-27 15:31:37.000000 polar_route-0.0.15/polar_route.egg-info/entry_points.txt
--rw-r--r--   0 jsmith     (501) staff       (20)        1 2022-10-18 09:50:41.000000 polar_route-0.0.15/polar_route.egg-info/not-zip-safe
--rw-r--r--   0 jsmith     (501) staff       (20)       97 2022-10-27 15:31:37.000000 polar_route-0.0.15/polar_route.egg-info/requires.txt
--rw-r--r--   0 jsmith     (501) staff       (20)       12 2022-10-27 15:31:37.000000 polar_route-0.0.15/polar_route.egg-info/top_level.txt
--rw-r--r--   0 jsmith     (501) staff       (20)      107 2022-10-27 15:31:37.849182 polar_route-0.0.15/setup.cfg
--rw-r--r--   0 jsmith     (501) staff       (20)     1673 2022-10-24 14:59:50.000000 polar_route-0.0.15/setup.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 14:04:35.759669 polar_route-0.1.0/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1081 2022-05-18 13:54:43.000000 polar_route-0.1.0/LICENSE
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       51 2022-11-01 08:06:54.000000 polar_route-0.1.0/MANIFEST.in
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4841 2023-04-19 14:04:35.759669 polar_route-0.1.0/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3710 2023-04-19 12:37:17.000000 polar_route-0.1.0/README.md
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 14:04:35.755669 polar_route-0.1.0/polar_route/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      731 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5571 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/cli.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    60611 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/crossing.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 14:04:35.755669 polar_route-0.1.0/polar_route/dataloaders/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1199 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/dataloader_interface.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    11372 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/factory.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 14:04:35.755669 polar_route-0.1.0/polar_route/dataloaders/scalar/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    25726 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/abstract_scalar.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3253 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/amsr.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1142 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/baltic_sea_ice.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1128 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/bsose_depth.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2034 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/bsose_sea_ice.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2804 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/density.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      908 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/gebco.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4263 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/icenet.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1008 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/modis.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      774 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/scalar_csv.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3043 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/scalar_grf.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7376 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/shape.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     3944 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/scalar/thickness.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 14:04:35.759669 polar_route-0.1.0/polar_route/dataloaders/vector/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/vector/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    26270 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/vector/abstract_vector.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1069 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/vector/baltic_current.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1331 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/vector/era5_wind.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1152 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/vector/north_sea_current.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1232 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/vector/oras5_current.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1172 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/vector/sose.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      790 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/vector/vector_csv.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2419 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/dataloaders/vector/vector_grf.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 14:04:35.759669 polar_route-0.1.0/polar_route/mesh_generation/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/mesh_generation/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4399 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/mesh_generation/aggregated_cellBox.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9879 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/mesh_generation/boundary.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    13950 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/mesh_generation/cellbox.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      367 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/mesh_generation/direction.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     9568 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/mesh_generation/environment_mesh.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2789 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/mesh_generation/jgrid_aggregated_cellbox.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     7503 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/mesh_generation/jgrid_cellbox.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5345 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/mesh_generation/mesh.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    22665 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/mesh_generation/mesh_builder.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2122 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/mesh_generation/metadata.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    13349 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/mesh_generation/neighbour_graph.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    32077 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/route_planner.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     8514 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/utils.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 14:04:35.759669 polar_route-0.1.0/polar_route/vessel_performance/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/vessel_performance/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1397 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/vessel_performance/abstract_vessel.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1448 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/vessel_performance/vessel_factory.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2977 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/vessel_performance/vessel_performance_modeller.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 14:04:35.759669 polar_route-0.1.0/polar_route/vessel_performance/vessels/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)    10968 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/vessel_performance/vessels/SDA.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/vessel_performance/vessels/__init__.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     5543 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/vessel_performance/vessels/abstract_ship.py
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1013 2023-04-19 12:37:17.000000 polar_route-0.1.0/polar_route/vessel_performance/vessels/underwater_vessel.py
+drwxrwxr-x   0 gecoomb   (1001) gecoomb   (1001)        0 2023-04-19 14:04:35.755669 polar_route-0.1.0/polar_route.egg-info/
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     4841 2023-04-19 14:04:35.000000 polar_route-0.1.0/polar_route.egg-info/PKG-INFO
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     2490 2023-04-19 14:04:35.000000 polar_route-0.1.0/polar_route.egg-info/SOURCES.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2023-04-19 14:04:35.000000 polar_route-0.1.0/polar_route.egg-info/dependency_links.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      210 2023-04-19 14:04:35.000000 polar_route-0.1.0/polar_route.egg-info/entry_points.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)        1 2022-09-01 09:10:15.000000 polar_route-0.1.0/polar_route.egg-info/not-zip-safe
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)      108 2023-04-19 14:04:35.000000 polar_route-0.1.0/polar_route.egg-info/requires.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       12 2023-04-19 14:04:35.000000 polar_route-0.1.0/polar_route.egg-info/top_level.txt
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)       38 2023-04-19 14:04:35.759669 polar_route-0.1.0/setup.cfg
+-rw-rw-r--   0 gecoomb   (1001) gecoomb   (1001)     1835 2023-04-19 12:37:17.000000 polar_route-0.1.0/setup.py
```

### Comparing `polar_route-0.0.15/LICENSE` & `polar_route-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polar_route-0.0.15/PKG-INFO` & `polar_route-0.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: polar_route
-Version: 0.0.15
-Summary: PolarRoute: Long-distance maritime polar route planning taking into account complex changing environmental conditions
-Home-page: https://www.github.com/antarctica
-Author: Jonathan Smith, Samuel Hall, George Coombs, James Byrne,  Michael Thorne, Maria Fox
-Author-email: jonsmi@bas.ac.uk
-Maintainer: Jonathan Smith, Samuel Hall, George Coombs, James Byrne,  Michael Thorne, Maria Fox
-Maintainer-email: jonsmi@bas.ac.uk
-License: MIT
-Platform: UNKNOWN
-Classifier: 
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Topic :: Scientific/Engineering
-Classifier: 
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-
 ![](logo.jpg)
 
 <a href="https://colab.research.google.com/drive/12D-CN10X7xAcXn_df0zNLHtdiiXxZVkz?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" alt="Colab">
 <a href="https://antarctica.github.io/PolarRoute/"><img src="https://img.shields.io/badge/Manual%20-github.io%2FPolarRoute%2F-red" alt="Manual Page">
 <a href="https://pypi.org/project/polar-route/"><img src="https://img.shields.io/pypi/v/polar-route" alt="PyPi">
 <a href="https://github.com/antarctica/PolarRoute/tags"><img src="https://img.shields.io/github/v/tag/antarctica/PolarRoute" alt="Release Tag"></a>
 <a href="https://github.com/antarctica/PolarRoute/issues"><img src="https://img.shields.io/github/issues/antarctica/PolarRoute" alt="Issues"></a>
@@ -46,20 +20,40 @@
 
  Pip: 
 ```
 pip install polar-route
 ```
 
 ## Required Data sources
-Polar-route has been built to work with a variety of open-source climactic data sources. 
-A list of supported data sources and there associated data-loaders is given in the 
+Polar-route has been built to work with a variety of open-source atmospheric and oceanographic data sources. 
+A list of supported data sources and their associated data-loaders is given in the 
 'Data Loaders' section of the manual
 
+## Documentation
+Sphinx is used to generate documentation for this project. The dependencies can be installed through pip:
+```
+pip install sphinx sphinx_markdown_builder sphinx_rtd_theme rinohtype
+```
+When updating the docs, run the following command within the PolarRoute directory to recompile.
+```
+sphinx-build -b html ./docs/source ./docs/html
+```
+Sometimes the cache needs to be cleared for internal links to update. If facing this problem, run this from the PolarRoute directory.
+```
+rm -r docs/build/.doctrees/
+```
 ## Developers
-Jonathan Smith, Samuel Hall, George Coombs, James Byrne,  Michael Thorne, Maria Fox
+Jonathan Smith, Samuel Hall, George Coombs, James Byrne,  Michael Thorne, Maria Fox, Harrison Abbot, Ayat Fekry
+
+## Collaboration
+We are currently assessing the best pratice for collaboration on the codebase, until then please contact [marfox@bas.ac.uk](marfox@bas.ac.uk) or [jonsmi@bas.ac.uk](jonsmi@bas.ac.uk) for further info.
+
 
 ## License
-This software is licensed under a MIT license. For more information please see the attached ``LICENSE`` file.
+This software is licensed under a MIT license, but request users cite our publication.  
+
+Jonathan D. Smith, Samuel Hall, George Coombs, James Byrne, Michael A. S. Thorne,  J. Alexander Brearley, Derek Long, Michael Meredith, Maria Fox,  (2022), Autonomous Passage Planning for a Polar Vessel, arXiv, https://arxiv.org/abs/2209.02389
+
+For more information please see the attached ``LICENSE`` file. 
 
 [version]: https://img.shields.io/PolarRoute/v/datadog-metrics.svg?style=flat-square
 [downloads]: https://img.shields.io/PolarRoute/dm/datadog-metrics.svg?style=flat-square
-
```

#### html2text {}

```diff
@@ -1,22 +1,8 @@
-Metadata-Version: 2.1 Name: polar_route Version: 0.0.15 Summary: PolarRoute:
-Long-distance maritime polar route planning taking into account complex
-changing environmental conditions Home-page: https://www.github.com/antarctica
-Author: Jonathan Smith, Samuel Hall, George Coombs, James Byrne, Michael
-Thorne, Maria Fox Author-email: jonsmi@bas.ac.uk Maintainer: Jonathan Smith,
-Samuel Hall, George Coombs, James Byrne, Michael Thorne, Maria Fox Maintainer-
-email: jonsmi@bas.ac.uk License: MIT Platform: UNKNOWN Classifier: Classifier:
-Development Status :: 3 - Alpha Classifier: Intended Audience :: Science/
-Research Classifier: Intended Audience :: System Administrators Classifier:
-License :: OSI Approved :: MIT License Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Topic :: Scientific/
-Engineering Classifier: Description-Content-Type: text/markdown Provides-Extra:
-tests ![](logo.jpg) [Open_In_Colab]_[Manual_Page]_[PyPi]_[Release_Tag]_[Issues]
+![](logo.jpg) [Open_In_Colab]_[Manual_Page]_[PyPi]_[Release_Tag]_[Issues]_
 [License]_#_PolarRoute_>_PolarRoute_is_a_long-distance_maritime_polar_route
 planning,_taking_into_account_complex_changing_environmental_conditions._The
 codebase_allows_the_construction_of_optimised_routes_through_three_main_stages:
 discrete_modelling_of_the_environmental_conditions_using_a_non-uniform_mesh,
 the_construction_of_mesh-optimal_paths,_and_physics_informed_path_smoothing._In
 order_to_account_for_different_vehicle_properties_we_construct_a_series_of_data
 driven_functions_that_can_be_applied_to_the_environmental_mesh_to_determine_the
@@ -24,14 +10,28 @@
 representing_these_quantities_graphically_and_geospatially._##_Installation_The
 PolarRoute_software_requires_GDAL_files_to_be_installed._The_PolarRoute
 software_can_be_installed_on_Windows_by_running_the_required_wheels_for_GDAL
 and_FIONA._MOre_information_can_be_found_in_the_manual_pages_linked_above._Once
 these_requirements_are_met_then_the_software_can_be_installed_by:_Github:_```
 python_setup.py_install_```_Pip:_```_pip_install_polar-route_```_##_Required
 Data_sources_Polar-route_has_been_built_to_work_with_a_variety_of_open-source
-climactic_data_sources._A_list_of_supported_data_sources_and_there_associated
-data-loaders_is_given_in_the_'Data_Loaders'_section_of_the_manual_##_Developers
+atmospheric_and_oceanographic_data_sources._A_list_of_supported_data_sources
+and_their_associated_data-loaders_is_given_in_the_'Data_Loaders'_section_of_the
+manual_##_Documentation_Sphinx_is_used_to_generate_documentation_for_this
+project._The_dependencies_can_be_installed_through_pip:_```_pip_install_sphinx
+sphinx_markdown_builder_sphinx_rtd_theme_rinohtype_```_When_updating_the_docs,
+run_the_following_command_within_the_PolarRoute_directory_to_recompile._```
+sphinx-build_-b_html_./docs/source_./docs/html_```_Sometimes_the_cache_needs_to
+be_cleared_for_internal_links_to_update._If_facing_this_problem,_run_this_from
+the_PolarRoute_directory._```_rm_-r_docs/build/.doctrees/_```_##_Developers
 Jonathan_Smith,_Samuel_Hall,_George_Coombs,_James_Byrne,_Michael_Thorne,_Maria
-Fox_##_License_This_software_is_licensed_under_a_MIT_license._For_more
-information_please_see_the_attached_``LICENSE``_file._[version]:_https://
-img.shields.io/PolarRoute/v/datadog-metrics.svg?style=flat-square_[downloads]:
-https://img.shields.io/PolarRoute/dm/datadog-metrics.svg?style=flat-square_
+Fox,_Harrison_Abbot,_Ayat_Fekry_##_Collaboration_We_are_currently_assessing_the
+best_pratice_for_collaboration_on_the_codebase,_until_then_please_contact_
+[marfox@bas.ac.uk](marfox@bas.ac.uk)_or_[jonsmi@bas.ac.uk](jonsmi@bas.ac.uk)
+for_further_info._##_License_This_software_is_licensed_under_a_MIT_license,_but
+request_users_cite_our_publication._Jonathan_D._Smith,_Samuel_Hall,_George
+Coombs,_James_Byrne,_Michael_A._S._Thorne,_J._Alexander_Brearley,_Derek_Long,
+Michael_Meredith,_Maria_Fox,_(2022),_Autonomous_Passage_Planning_for_a_Polar
+Vessel,_arXiv,_https://arxiv.org/abs/2209.02389_For_more_information_please_see
+the_attached_``LICENSE``_file._[version]:_https://img.shields.io/PolarRoute/v/
+datadog-metrics.svg?style=flat-square_[downloads]:_https://img.shields.io/
+PolarRoute/dm/datadog-metrics.svg?style=flat-square_
```

### Comparing `polar_route-0.0.15/polar_route/crossing.py` & `polar_route-0.1.0/polar_route/crossing.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,14 +4,15 @@
      In the section below we will go through, stage by stage, how the crossing point is determined and the methods
      used within the classes.
 
 """
 import copy
 import pandas as pd
 import numpy as np
+import pyproj
 np.seterr(divide='ignore', invalid='ignore')
 
 
 class NewtonianDistance:
     """The summary line for a class docstring should fit on one line.
 
     If the class has public attributes, they may be documented here
@@ -48,19 +49,23 @@
             param3 (:obj:`list` of :obj:`str`): Description of `param3`.
 
         """
         # Cell information
         self.source_graph     = source_graph
         self.neighbour_graph  = neighbour_graph
 
+        # Case indices
+        self.indx_type = np.array([1, 2, 3, 4, -1, -2, -3, -4])
+
         # Inside the code the base units are m/s. Changing the units of the inputs to match
+        indx = np.where(self.indx_type==case)[0][0]
         self.unit_shipspeed  = unit_shipspeed
         self.unit_time       = unit_time
-        self.source_speed    = self._unit_speed(self.source_graph['Speed'])
-        self.neighbour_speed = self._unit_speed(self.neighbour_graph['Speed'])
+        self.source_speed    = self._unit_speed(self.source_graph['speed'][indx])
+        self.neighbour_speed = self._unit_speed(self.neighbour_graph['speed'][indx])
         self.case            = case
 
         if zerocurrents:
             self.zero_current_factor = 0.0
         else:
             self.zero_current_factor = 1.0
 
@@ -85,22 +90,27 @@
         y0 = (Y*x)/(x+a)
         if self.debugging:
             print('---Initial y={:.2f}'.format(y0))
         improving = True
         iterartion_num = 0
         while improving:
             F,dF,X1,X2,t1,t2  = f(y0,x,a,Y,u1,v1,u2,v2,s1,s2)
+            if F==np.inf:
+                return np.nan,np.inf  
+
             if self.debugging:
                 print('---Iteration {}: y={:.2f}; F={:.5f}; dF={:.2f}'\
                       .format(iterartion_num,y0,F,dF))
             y0  = y0 - (F/dF)
             improving = abs((F/dF)/(X1*X2)) > self.optimizer_tol
             iterartion_num+=1
             if iterartion_num>1000:
                 raise Exception('Newton not able to converge')
+            
+
         return y0,self._unit_time(np.array([t1,t2]))
 
     def _unit_speed(self,val):
         '''
             FILL
         '''
         if not isinstance(val,type(None)):
@@ -122,25 +132,14 @@
             val = val/(60*60.)
         elif self.unit_time == 'min':
             val = val/(60.)
         elif self.unit_time == 's':
             val = val
         return val
 
-    def waypoint_correction(self,Wp,Cp):
-        '''
-            FILL
-        '''
-        x = (Cp[0]-Wp[0])*self.m_long*np.cos(Wp[1]*(np.pi/180))
-        y = (Cp[1]-Wp[1])*self.m_lat
-        Su  = self.source_graph['Vector_x']*self.zero_current_factor
-        Sv  = self.source_graph['Vector_y']*self.zero_current_factor
-        Ssp = self.source_speed
-        traveltime = self._traveltime_in_cell(x,y,Su,Sv,Ssp)
-        return self._unit_time(traveltime)
 
     def _F(self,y,x,a,Y,u1,v1,u2,v2,s1,s2):
         '''
             FILL
         '''
         C1 = s1**2 - u1**2 - v1**2
         C2 = s2**2 - u2**2 - v2**2
@@ -153,14 +152,17 @@
             X1 = np.sqrt(X1ns)
         X2ns = D2**2 + C2*(a**2 + (Y-y)**2)
         if X2ns < 0:
             X2 = -1
         else:
             X2 = np.sqrt(X2ns)
 
+        if X1 < 0 or X2 < 0:
+            return np.inf,np.inf,np.inf,np.inf,np.inf,np.inf
+
         F  = X2*(y-((v1*(X1-D1))/C1)) + X1*(y-Y+((v2*(X2-D2))/C2))
 
         dD1 = v1
         dD2 = -v2
         if X1 == 0:
             dX1 = 0
         else:
@@ -199,17 +201,31 @@
                 else:
                     traveltime = dist * dist / (2 * dotprod)
                     return traveltime
 
         traveltime = (np.sqrt(dotprod**2 + (dist**2)*diffsqrs) - dotprod)/diffsqrs
         if traveltime < 0:
             traveltime = np.inf
-            #raise Exception('Newton Corner Cases returning Zero Traveltime - ISSUE')
+            # print(traveltime,xdist,ydist,U,V,S)
+            # raise Exception('Newton Corner Cases returning Zero Traveltime - ISSUE')
         return traveltime
 
+    def waypoint_correction(self,Wp,Cp):
+        '''
+            FILL
+        '''
+        x = (Cp[0]-Wp[0])*self.m_long*np.cos(Wp[1]*(np.pi/180))
+        y = (Cp[1]-Wp[1])*self.m_lat
+        Su  = self.source_graph['Vector_x']*self.zero_current_factor
+        Sv  = self.source_graph['Vector_y']*self.zero_current_factor
+        Ssp = self.source_speed
+        traveltime = self._traveltime_in_cell(x,y,Su,Sv,Ssp)
+        return self._unit_time(traveltime)
+
+
     def _longitude(self):
         '''
             FILL
         '''
 
         if self.case==2:
             ptvl = 1.0
@@ -237,30 +253,53 @@
 
         x = s_dcx*self.m_long*np.cos(s_cy*(np.pi/180))
         a = n_dcx*self.m_long*np.cos(n_cy*(np.pi/180))
         Y = ptvl*(n_cy-s_cy)*self.m_lat
 
         # Optimising to determine the y-value of the crossing point
         y,TravelTime = self._newton_optimisation(self._F,x,a,Y,Su,Sv,Nu,Nv,Ssp,Nsp)
+        if np.isnan(y) or TravelTime[0] < 0 or TravelTime[1] < 0:
+            TravelTime  = [np.inf,np.inf]
+            CrossPoints = [np.nan,np.nan]
+            CellPoints  = [np.nan,np.nan]
+            return TravelTime,CrossPoints,CellPoints
+
+        
         CrossPoints = (s_cx+ptvl*s_dcx,\
                        s_cy+ptvl*y/self.m_lat)
         CellPoints  = [n_cx,n_cy]
 
+
+        # Checking Crossing Ponint possible
+        # Defining the min and max of the start and end cells
+        smin = s_cy-s_dcy 
+        smax = s_cy+s_dcy 
+        emin = n_cy-n_dcy
+        emax = n_cy+n_dcy
+        vmin = np.max([smin,emin])
+        vmax = np.min([smax,emax])
+        if (CrossPoints [1] < vmin) or (CrossPoints[1] > vmax):
+            TravelTime  = [np.inf,np.inf]
+            CrossPoints = [np.nan,np.nan]
+            CellPoints  = [np.nan,np.nan]
+
+
         return TravelTime,CrossPoints,CellPoints
 
     def _latitude(self):
         '''
             FILL
         '''
 
         if self.case==4:
             ptvl = 1.0
         else:
             ptvl = -1.0
 
+
         s_cx  = self.source_graph['cx']
         s_cy  = self.source_graph['cy']
         s_dcx = self.source_graph['dcx']
         s_dcy = self.source_graph['dcy']
         n_cx  = self.neighbour_graph['cx']
         n_cy  = self.neighbour_graph['cy']
         n_dcx = self.neighbour_graph['dcx']
@@ -268,29 +307,58 @@
 
 
         Su = -1*ptvl*self.source_graph['Vector_y']*self.zero_current_factor
         Sv = ptvl*self.source_graph['Vector_x']*self.zero_current_factor
         Nu = -1*ptvl*self.neighbour_graph['Vector_y']*self.zero_current_factor
         Nv = ptvl*self.neighbour_graph['Vector_x']*self.zero_current_factor
 
+
         Ssp=self.source_speed
         Nsp=self.neighbour_speed
 
         x = s_dcy*self.m_lat
         a = n_dcy*self.m_lat
         Y = ptvl*(n_cx-s_cx)*self.m_long*np.cos((n_cy+s_cy)*(np.pi/180)/2.0)
-
+        
+        
         y,TravelTime   = self._newton_optimisation(self._F,x,a,Y,Su,Sv,Nu,Nv,Ssp,Nsp)
-        clon = s_cx  + ptvl*y/(self.m_long*np.cos((n_cy+\
-               s_cy)*(np.pi/180)/2.0))
+        if np.isnan(y) or TravelTime[0] < 0 or TravelTime[1] < 0:
+            TravelTime  = [np.inf,np.inf]
+            CrossPoints = [np.nan,np.nan]
+            CellPoints  = [np.nan,np.nan]
+            return TravelTime,CrossPoints,CellPoints
+
+
+        clon = s_cx  + ptvl*y/(self.m_long*np.cos((n_cy+s_cy)*(np.pi/180)/2.0))
         clat = s_cy + -1*ptvl*s_dcy
 
         CrossPoints = (clon,clat)
         CellPoints  = [n_cx,n_cy]
 
+
+        # Checking Crossing Ponint possible
+        # Defining the min and max of the start and end cells
+        smin = s_cx-s_dcx 
+        smax = s_cx+s_dcx 
+        emin = n_cx-n_dcx
+        emax = n_cx+n_dcx
+        vmin = np.max([smin,emin])
+        vmax = np.min([smax,emax])
+        if (CrossPoints [0] < vmin) or (CrossPoints[0] > vmax):
+            TravelTime  = [np.inf,np.inf]
+            CrossPoints = [np.nan,np.nan]
+            CellPoints  = [np.nan,np.nan]
+
+        # if TravelTime[0] < 0 or TravelTime[1] < 0:
+        #     TravelTime  = [np.inf,np.inf]
+        #     CrossPoints = [np.nan,np.nan]
+        #     CellPoints  = [np.nan,np.nan]
+        #     return TravelTime,CrossPoints,CellPoints
+
+
         return TravelTime,CrossPoints,CellPoints
 
 
     def _corner(self):
         '''
             FILL
         '''
@@ -303,52 +371,73 @@
         n_cx  = self.neighbour_graph['cx']
         n_cy  = self.neighbour_graph['cy']
         n_dcx = self.neighbour_graph['dcx']
         n_dcy = self.neighbour_graph['dcy']
 
 
 
-        # Given the determine the postive and negative position relative to centre
+        # Given the case determine the postive and negative position relative to centre
         if self.case==1:
             ptvX = 1.0
             ptvY = 1.0
         elif self.case==-1:
             ptvX = -1.0
             ptvY = -1.0
         elif self.case==3:
             ptvX = 1.0
             ptvY = -1.0
         elif self.case==-3:
             ptvX = -1.0
             ptvY = 1.0
 
-        dx1 = s_dcx*self.m_long*np.cos(s_cy*(np.pi/180))
-        dx2 = n_dcx*self.m_long*np.cos(n_cy*(np.pi/180))
-        dy1 = s_dcy*self.m_lat
-        dy2 = n_dcy*self.m_lat
+        # dx1 = s_dcx*self.m_long*np.cos(s_cy*(np.pi/180))
+        # dx2 = n_dcx*self.m_long*np.cos(n_cy*(np.pi/180))
+        # dy1 = s_dcy*self.m_lat
+        # dy2 = n_dcy*self.m_lat
+
+        # # Currents in Cells
+        # Su = ptvX*self.source_graph['Vector_x']*self.zero_current_factor
+        # Sv = ptvY*self.source_graph['Vector_y']*self.zero_current_factor
+        # Nu = ptvX*self.neighbour_graph['Vector_x']*self.zero_current_factor
+        # Nv = ptvY*self.neighbour_graph['Vector_y']*self.zero_current_factor
+
+
+        dx1 = ptvX*s_dcx*self.m_long*np.cos(s_cy*(np.pi/180))
+        dx2 = ptvX*n_dcx*self.m_long*np.cos(n_cy*(np.pi/180))
+        dy1 = ptvY*s_dcy*self.m_lat
+        dy2 = ptvY*n_dcy*self.m_lat
 
         # Currents in Cells
-        Su = ptvX*self.source_graph['Vector_x']*self.zero_current_factor
-        Sv = ptvY*self.source_graph['Vector_y']*self.zero_current_factor
-        Nu = ptvX*self.neighbour_graph['Vector_x']*self.zero_current_factor
-        Nv = ptvY*self.neighbour_graph['Vector_y']*self.zero_current_factor
+        Su = self.source_graph['Vector_x']*self.zero_current_factor
+        Sv = self.source_graph['Vector_y']*self.zero_current_factor
+        Nu = self.neighbour_graph['Vector_x']*self.zero_current_factor
+        Nv = self.neighbour_graph['Vector_y']*self.zero_current_factor
+
+
 
         # Vehicles Speeds in Cells
         Ssp = self.source_speed; Nsp = self.neighbour_speed
 
         # Determining the crossing point as the corner of the case
         CrossPoints = [s_cx+ptvX*s_dcx,\
                        s_cy+ptvY*s_dcy]
         CellPoints  = [n_cx,n_cy]
 
         # Determining traveltime
         t1 = self._traveltime_in_cell(dx1,dy1,Su,Sv,Ssp)
         t2 = self._traveltime_in_cell(dx2,dy2,Nu,Nv,Nsp)
         TravelTime  = self._unit_time(np.array([t1,t2]))
 
+        if TravelTime[0] < 0 or TravelTime[1] < 0:
+            TravelTime  = [np.inf,np.inf]
+            CrossPoints = [np.nan,np.nan]
+            CellPoints  = [np.nan,np.nan]
+            return TravelTime,CrossPoints,CellPoints
+
+
         return TravelTime,CrossPoints,CellPoints
 
 
     def value(self):
         '''
             FILLE
         '''
@@ -363,111 +452,283 @@
         else:
             print('---> Issue with cell (Xsc,Ysc)={:.2f};{:.2f}'.\
                 format(self.source_graph['cx'],self.source_graph['cy']))
             TravelTime  = [np.inf,np.inf]
             CrossPoints = [np.nan,np.nan]
             CellPoints  = [np.nan,np.nan]
 
-        return TravelTime, CrossPoints, CellPoints
+        return TravelTime, CrossPoints, CellPoints, self.case
 
 
 # ===================================================================================================
 # ===================================================================================================
 # ===================================================================================================
 # ===================================================================================================
 # ===================================================================================================
 # ===================================================================================================
 
 
 class NewtonianCurve:
-    def __init__(self,neighbour_graph,config,unit_shipspeed='km/hr',unit_time='days',debugging=False,maxiter=1000,pathIter=5,optimizer_tol=1e-3,minimumDiff=1e-3,zerocurrents=True):
+    def __init__(self,neighbour_graph,config,unit_shipspeed='km/hr',unit_time='days', objective_func='traveltime',debugging=False,maxiter=1000,minimumDiff=1e-3,zerocurrents=False):
         '''
-            FILL
+            Applys path smoothing to input neighbourhood graph constructed during the dijkstra run.
+
+            Args:
+                neigbour_graph: Dijkstra based neighbourhood graph (Pandas DataFrame)
+                config: Input path configuration
+            
+            Opt Args:
+                unit_speed: Input unit speed type from mesh (Default:'km/hr')
+                unit_time: Input unit time to output (Default:'km/hr')
+                objective_func: Objective function to apply path smoothing relative. 
+                    This should be the same as used in Dijkstra. (Default:'traveltime')
+                
+                maxiter: Maximum number of iterations for the path smoothing (Default:1000)
+                minimumDiff: Tolerence for the path smoothing for the maximum deg distance between two points (Default:1e-3)
+                zerocurrents: Boolean to Zero currents for path smoothing. Used for debugging cases only (Default:False)
+
         '''
         # Passing the Dijkstra Graph
         self.neighbour_graph = copy.copy(neighbour_graph)
 
         # Passing the optional Information
         self.config = config
 
         
         # Inside the code the base units are m/s. Changing the units of the inputs to match
         self.unit_shipspeed = unit_shipspeed
         self.unit_time      = unit_time
 
+
+        self.objective_func = objective_func
         
         # Information for distance metrics
         self.R              = 6371.*1000
 
+        # Case indices
+        self.indx_type = np.array([1, 2, 3, 4, -1, -2, -3, -4])
+
         # Optimisation Information
         self.maxiter       = maxiter
-        self.pathIter      = pathIter
-        self.optimizer_tol = optimizer_tol
         self.minimumDiff   = minimumDiff
         self._epsilon      = 1e-3
 
 
         # Optimisation Information
         self.m_long  = 111.321*1000
         self.m_lat   = 111.386*1000.
 
         # For Debugging purposes 
         self.debugging     = debugging
 
-        if self.debugging:
-            self.debugFile1 = open("debugFil.txt", "w")  # append mode
-            self.debugFile1.write("Today \n")
-
-        self.id = 0
-
         # zeroing currents if flagged
         if zerocurrents:
             self.zc = 0.0
         else:
             self.zc = 1.0
 
+
+        self.previous_horeshoes = []
+
     def _unit_speed(self,Val):
         '''
-            FILL
+            Applying unit speed for an input type.
         '''
         if self.unit_shipspeed == 'km/hr':
             Val = Val*(1000/(60*60))
         if self.unit_shipspeed == 'knots':
             Val = (Val*0.51)
         return Val
 
     def _unit_time(self,Val):
         '''
-            FILL
+            Applying Unit time for a specific input type
         '''
         if self.unit_time == 'days':
             Val = Val/(60*60*24)
         elif self.unit_time == 'hr':
             Val = Val/(60*60)
         elif self.unit_time == 'min':
             Val = Val/(60)
         elif self.unit_time == 's':
             Val = Val
         return Val
 
 
-    def _calXDist(self,start_long,end_long):
+    def _calXDist(self,start_long,end_long,centralLat):
         '''
-            FILL
+            Calculate the X Distance
         '''
-        return (end_long - start_long)*self.m_long#*np.cos(centralLat)
+        return (end_long - start_long)*self.m_long#*np.cos(centralLat*(np.pi/180))
     def _calYDist(self,start_lat,end_lat):
         '''
-            FILL
+            Calculate the Y Distance
         '''
         return (end_lat-start_lat)*self.m_lat
 
+    
+    def _traveltime_in_cell(self,xdist,ydist,U,V,S):
+        '''
+            Determine the traveltime within cell
+        '''
+        dist  = np.sqrt(xdist**2 + ydist**2)
+        cval  = np.sqrt(U**2 + V**2)
+
+        dotprod  = xdist*U + ydist*V
+        diffsqrs = S**2 - cval**2
+
+        # if (dotprod**2 + diffsqrs*(dist**2) < 0)
+        if diffsqrs == 0.0:
+            if dotprod == 0.0:
+                return np.inf
+                #raise Exception(' ')
+            else:
+                if ((dist**2)/(2*dotprod))  <0:
+                    return np.inf
+                    #raise Exception(' ')
+                else:
+                    traveltime = dist * dist / (2 * dotprod)
+                    return traveltime
+
+        traveltime = (np.sqrt(dotprod**2 + (dist**2)*diffsqrs) - dotprod)/diffsqrs
+        if traveltime < 0:
+            traveltime = np.inf
+        return self._unit_time(traveltime), dist
+
+
+    def _case_from_angle(self,start,end):
+        """
+            Determine the direction of travel between two points in the same cell and return the associated case
+
+            Args:
+                start (list): the coordinates of the start point within the cell
+                end (list):  the coordinates of the end point within the cell
+
+            Returns:
+                case (int): the case to use to select variable values from a list
+        """
+
+        direct_vec = [end[0]-start[0], end[1]-start[1]]
+        direct_ang = np.degrees(np.arctan2(direct_vec[0], direct_vec[1]))
+
+        case = None
+
+        if -22.5 <= direct_ang < 22.5:
+            case = -4
+        elif 22.5 <= direct_ang < 67.5:
+            case = 1
+        elif 67.5 <= direct_ang < 112.5:
+            case = 2
+        elif 112.5 <= direct_ang < 157.5:
+            case = 3
+        elif 157.5 <= abs(direct_ang) <= 180:
+            case = 4
+        elif -67.5 <= direct_ang < -22.5:
+            case = -3
+        elif -112.5 <= direct_ang < -67.5:
+            case = -2
+        elif -157.5 <= direct_ang < -112.5:
+            case = -1
+
+        return case
+
+
+    def _waypoint_correction(self,path_requested_variables,source_graph,Wp,Cp):
+        '''
+            Determine within cell parameters for a source and end point on the edge
+        '''
+        m_long  = 111.321*1000
+        m_lat   = 111.386*1000
+        x = (Cp[0]-Wp[0])*m_long*np.cos(Wp[1]*(np.pi/180))
+        y = (Cp[1]-Wp[1])*m_lat
+        case = self._case_from_angle(Cp,Wp)
+        Su  = source_graph['Vector_x']*self.zc
+        Sv  = source_graph['Vector_y']*self.zc
+        Ssp = self._unit_speed(source_graph['speed'][case])
+        traveltime, distance = self._traveltime_in_cell(x,y,Su,Sv,Ssp)
+
+
+        segment_values = {}
+        for var in path_requested_variables.keys():
+            if var=='distance':
+                segment_values[var] = distance
+            elif var=='traveltime':
+                segment_values[var] = traveltime
+            elif var=='cell_index':
+                segment_values[var] = int(source_graph.name)
+            else:
+                if var in source_graph.keys():
+                    # Determining the objective value information
+                    if type(source_graph[var]) == list:
+                        objective_rate_value = source_graph[var][case]
+                    else:
+                        objective_rate_value = source_graph[var]
+                    if path_requested_variables[var]['processing'] is None:
+                        segment_values[var] = objective_rate_value
+                    else:
+                        segment_values[var] = traveltime*objective_rate_value
+
+        return segment_values, case
+
+    def objective_function(self,Points):
+        '''
+            Given a series of points determine the path based values along the path.
+        '''
+
+        # Determining the important variables to return for the paths
+        required_path_variables = {'distance':{'processing':'cumsum'},
+                                   'traveltime':{'processing':'cumsum'},
+                                   'datetime':{'processing':'cumsum'},
+                                   'cell_index':{'processing':None},
+                                   'speed':{'processing':None},
+                                   'fuel':{'processing':'cumsum'}}
+        path_requested_variables = {} #self.config['Route_Info']['path_variables']
+        path_requested_variables.update(required_path_variables)
+
+
+
+        # Initialising zero arrays for the path variables 
+        variables =  {}    
+        for var in path_requested_variables:
+            variables[var] ={}
+            variables[var]['path_values'] = np.zeros(len(Points))
+
+
+        # Looping over the path and determining the variable information
+        for ii in range(len(Points)-1):
+
+            # Determining the cellbox to determine path values from
+            cellbox = Points.iloc[ii]['cellEnd']
+            Wp = Points.iloc[ii][['cx','cy']].to_numpy()
+            Cp = Points.iloc[ii+1][['cx','cy']].to_numpy()
+            
+            # Determining the value for the variable for the segment of the path and the corresponding case
+            segment_variable, segment_case = self._waypoint_correction(path_requested_variables,cellbox,Wp,Cp)
+
+            # Adding that value for the segment along the paths
+            for var in segment_variable:
+                if type(segment_variable[var]) == list:
+                    variables[var]['path_values'][ii+1] = segment_variable[var][segment_case]
+                else:
+                    variables[var]['path_values'][ii+1] = segment_variable[var]
+
+
+        # Applying processing to all path values
+        for var in variables.keys():
+            processing_type = path_requested_variables[var]['processing']
+            if type(processing_type) == type(None):
+                continue
+            elif processing_type == 'cumsum':
+                variables[var]['path_values'] = np.cumsum(variables[var]['path_values'])
+
+        return variables
+
     def _long_case(self):
         '''
-            FILL
+            Longitude based smoothing
         '''
         def NewtonOptimisationLong(f,y0,x,a,Y,u1,v1,u2,v2,speed_s,speed_e,R,λ_s,φ_r):
                 tryNum=1
                 iter=0
                 improving=True
                 while improving:  
                     F,dF,X1,X2  = f(y0,x,a,Y,u1,v1,u2,v2,speed_s,speed_e,R,λ_s,φ_r)
@@ -496,43 +757,52 @@
                             else:
                                 y0 = (tryNum-3)*-Y
                     if iter > 1000:
                         raise Exception('Newton Curve Issue')
                 return y0
 
         def _F(y,x,a,Y,u1,v1,u2,v2,speed_s,speed_e,R,λ_s,φ_r):
-            θ  = (y/R + λ_s*(np.pi/180))
+            ρ = (λ_s+φ_r)/2.0
+            ϕ_min = min(λ_s,φ_r) 
+            if λ_s > φ_r:
+                ϕ_l   = ρ
+                ϕ_r   = (ϕ_min+ρ)/2
+            else:
+                ϕ_l   = (ϕ_min+ρ)/2
+                ϕ_r   = ρ
+
+            θ  = (y/(2*R) + ϕ_l) #(y/R + λ_s)
             zl = x*np.cos(θ)
-            ψ  = (-(Y-y)/R + φ_r*(np.pi/180))
+            ψ  = ((Y-y)/(2*R) + ϕ_r) #((Y-y)/R + φ_r)
             zr = a*np.cos(ψ)
 
             C1  = speed_s**2 - u1**2 - v1**2
             C2  = speed_e**2 - u2**2 - v2**2
             D1  = zl*u1 + y*v1
             D2  = zr*u2 + (Y-y)*v2
             X1  = np.sqrt(D1**2 + C1*(zl**2 + y**2))
             X2  = np.sqrt(D2**2 + C2*(zr**2 + (Y-y)**2))
 
-            dzr = -zr*np.sin(ψ)/R
-            dzl = -zl*np.sin(θ)/R
+            dzr = -a*np.sin(ψ)/(2*R)#-zr*np.sin(ψ)/R
+            dzl = -x*np.sin(θ)/(2*R)#-zl*np.sin(θ)/R
 
             dD1 = dzl*u1 + v1
             dD2 = dzr*u2 - v2
             dX1 = (D1*v1 + C1*y + dzl*(D1*u1 + C1*zl))/X1
             dX2 = (-v2*D2 - C2*(Y-y) + dzr*(D2*u2 + C2*zr))/X2     
 
             zr_term = (zr - (X2 - D2)*u2/C2)
             zl_term = (zl - (X1 - D1)*u1/C1)
 
             F = (X1+X2)*y - v1*(X1-D1)*X2/C1 - (Y - v2*(X2-D2)/C2)*X1 + dzr*zr_term*X1 + dzl*zl_term*X2
 
             dF = (X1+X2) + y*(dX1 + dX2) - (v1/C1)*(dX2*(X1-D1) + X2*(dX1-dD1))\
                 - Y*dX1 + (v2/C2)*(dX1*(X2-D2) + X1*(dX2-dD2))\
-                - (zr/(R**2))*zr_term*X1\
-                - (zl/(R**2))*zl_term*X2\
+                - (zr/(4*(R**2)))*zr_term*X1\
+                - (zl/(4*(R**2)))*zl_term*X2\
                 + dzr*(dzr-u2*(dX2-dD2))/C2*X1\
                 + dzl*(dzl-u1*(dX1-dD1))/C1*X2\
                 + dzr*zr_term*dX1 + dzl*zl_term*dX2
 
             return F,dF,X1,X2
 
         Sp   = tuple(self.triplet[['cx','cy']].iloc[0])
@@ -545,33 +815,33 @@
         cell_e_v = self.neighbour_graph.loc[self.triplet.iloc[1]['cellEnd'].name,'Vector_y']
 
         if self.triplet.iloc[1].case == 2:   
             sgn  = 1
         else:
             sgn  = -1
 
-        λ_s  = Sp[1]
-        φ_r  = Np[1]
+        λ_s  = Sp[1]*(np.pi/180)
+        φ_r  = Np[1]*(np.pi/180)
 
-        x           = sgn*self._calXDist(Sp[0],Cp[0])
-        a           = sgn*self._calXDist(Cp[0],Np[0])
+        x           = sgn*self._calXDist(Sp[0],Cp[0],Cp[1])
+        a           = sgn*self._calXDist(Cp[0],Np[0],Cp[1])
         Y           = (Np[1]-Sp[1])*self.m_lat
         y0          = Y/2
         u1          = sgn*self.zc*cell_s_u; v1 = self.zc*cell_s_v
         u2          = sgn*self.zc*cell_e_u; v2 = self.zc*cell_e_v
         y           = NewtonOptimisationLong(_F,y0,x,a,Y,u1,v1,u2,v2,self.speed_s,self.speed_e,self.R,λ_s,φ_r)
 
         # Updating the crossing points
         self.triplet['cx'].iloc[1] = Cp[0]
         self.triplet['cy'].iloc[1] = Sp[1] + y/self.m_lat
 
 
     def _lat_case(self):
         '''
-            FILL
+            Latitude based smoothing
         '''
         def NewtonOptimisationLat(f,y0,x,a,Y,u1,v1,u2,v2,speed_s,speed_e,R,λ,θ,ψ):
                 tryNum=1
                 iter=0
                 improving=True
                 while improving:  
                     F,dF,X1,X2  = f(y0,x,a,Y,u1,v1,u2,v2,speed_s,speed_e,R,λ,θ,ψ)
@@ -602,16 +872,18 @@
                         raise Exception('Newton Curve Issue')
                 return y0
 
         def _F(y,x,a,Y,u1,v1,u2,v2,speed_s,speed_e,R,λ,θ,ψ):
             λ   = λ*(np.pi/180)
             ψ   = ψ*(np.pi/180)
             θ   = θ*(np.pi/180)
-            r1  = np.cos(λ)/np.cos(θ)
-            r2  = np.cos(ψ)/np.cos(θ)
+            #r1  = np.cos(λ)/np.cos(θ)
+            r1  = np.cos((θ + 3*λ)/4)/np.cos(θ)
+            #r2  = np.cos(ψ)/np.cos(θ)
+            r2  = np.cos((θ + 3*ψ)/4)/np.cos(θ)
 
             d1  = np.sqrt(x**2 + (r1*y)**2)
             d2  = np.sqrt(a**2 + (r2*(Y-y))**2)
             C1  = speed_s**2 - u1**2 - v1**2
             C2  = speed_e**2 - u2**2 - v2**2
             D1  = x*u1 + r1*v1*y
             D2  = a*u2 + r2*v2*(Y-y)
@@ -662,28 +934,43 @@
 
         self.triplet['cx'].iloc[1] = Sp[0] + sgn*y/(self.m_long*np.cos(Cp[1]*(np.pi/180)))
         self.triplet['cy'].iloc[1] = Cp[1]
 
 
     def _corner_case(self):
         '''
-            FILL
+            If a point lies on the corner of a cell how to introduce new corner edges.
         '''
         # Separting out the Long/Lat of each of the points
         Xs,Ys = tuple(self.triplet.iloc[0][['cx','cy']])
         Xc,Yc = tuple(self.triplet.iloc[1][['cx','cy']])
         Xe,Ye = tuple(self.triplet.iloc[2][['cx','cy']])
 
         # === 1. Assess the cells that are shared commonly in the corner case ====
         sourceNeighbourIndices = self.triplet.iloc[1]['cellStart']
         endNeighbourIndices    = self.triplet.iloc[1]['cellEnd']
     
         commonIndices = list(set(sourceNeighbourIndices['neighbourIndex']).intersection(endNeighbourIndices['neighbourIndex']))
         CornerCells   = self.neighbour_graph.loc[commonIndices]
-        Y_line = ((Ye-Ys)/(Xe-Xs))*(Xc-Xs) + Ys
+
+
+        # Arc Crossing Point
+        def great_circle_lat(start_lat, start_long, end_lat, end_long,mid_long):
+            # calculate distance between points
+            g = pyproj.Geod(ellps='WGS84')
+            (az12, az21, dist) = g.inv(start_long, start_lat, end_long, end_lat)
+            # calculate line string along path with segments <= 1 km
+            lonlats = np.array(g.npts(start_long, start_lat, end_long, end_lat,50000))
+            diff    = abs(lonlats[:,0]-mid_long)
+            mid_lat = lonlats[np.argmin(diff),1]
+            return mid_lat,np.min(diff)
+        Y_line,diff = great_circle_lat(Ys,Xs,Ye,Xe,Xc)
+        # if diff > 1e-3:
+        #     raise Exception('Corner Case Issue - Great-Circle Crossing too coarse')
+
 
         try:
             if Yc >= Y_line:
                 newCell = CornerCells.loc[CornerCells['cy'].idxmin()]
                 if newCell.cy > Yc:
                     return
             elif Yc < Y_line:
@@ -691,65 +978,90 @@
                 if newCell.cy < Yc:
                     return
             # === 3. Return the path crossing points and cell indices
 
             firstCrossingPoint  = np.array(sourceNeighbourIndices['neighbourCrossingPoints'])[np.where(np.array(sourceNeighbourIndices['neighbourIndex'])==newCell.name)[0][0],:]
             secondCrossingPoint = np.array(newCell['neighbourCrossingPoints'])[np.where(np.array(newCell['neighbourIndex'])==endNeighbourIndices.name)[0][0],:]
         except:
-            self.triplet = copy.deepcopy(self.org_triplet)
             return
-
-        # Adding in the new crossing Point
-        newP = pd.Series(name=self.triplet.iloc[1].name+1,dtype='object')
-        newP['cx']        = secondCrossingPoint[0]
-        newP['cy']        = secondCrossingPoint[1]
-        newP['cellStart'] = newCell
-        newP['cellEnd']   = copy.deepcopy(self.triplet['cellEnd'].iloc[1])
-        newP['case']      = newP['cellStart']['case'][np.where(np.array(newP['cellStart']['neighbourIndex'])==newP['cellEnd'].name)[0][0]]
-
-
-        # Updating the origional crossing point
-        self.triplet['cx'].iloc[1]      = firstCrossingPoint[0]
-        self.triplet['cy'].iloc[1]      = firstCrossingPoint[1]
-        self.triplet['cellEnd'].iloc[1] = newCell 
-        self.triplet['case'].iloc[1]    = self.triplet['cellStart'].iloc[1]['case'][np.where(np.array(self.triplet['cellStart'].iloc[1]['neighbourIndex'])==newCell.name)[0][0]]
+        
+        if np.isnan(np.concatenate([firstCrossingPoint,secondCrossingPoint]).astype(float)).any():
+            return
 
 
-        # Adding the new crossing point to the triplet
-        self.newP = newP
+        # Crossing point 1
+        Pcrp1 = copy.deepcopy(self.triplet.iloc[0])
+        # Crossing point 2
+        Pcrp2 = pd.Series(name=self.triplet.iloc[1].name,dtype='object')
+        Pcrp2['cx']        = firstCrossingPoint[0]
+        Pcrp2['cy']        = firstCrossingPoint[1]
+        Pcrp2['cellStart'] = copy.deepcopy(self.triplet['cellStart'].iloc[1])
+        Pcrp2['cellEnd']   = copy.deepcopy(newCell)
+        Pcrp2['case']      = self.triplet['cellStart'].iloc[1]['case'][np.where(np.array(self.triplet['cellStart'].iloc[1]['neighbourIndex'])==newCell.name)[0][0]]
+
+        # Crossing point 3
+        Pcrp3 = pd.Series(name=self.triplet.iloc[1].name+1,dtype='object')
+        Pcrp3['cx']        = secondCrossingPoint[0]
+        Pcrp3['cy']        = secondCrossingPoint[1]
+        Pcrp3['cellStart'] = copy.deepcopy(newCell)
+        Pcrp3['cellEnd']   = copy.deepcopy(self.triplet['cellEnd'].iloc[1])
+        Pcrp3['case']      = Pcrp3['cellStart']['case'][np.where(np.array(Pcrp3['cellStart']['neighbourIndex'])==Pcrp3['cellEnd'].name)[0][0]]
+        # Crossing point 4
+        Pcrp4 = copy.deepcopy(self.triplet.iloc[2])
+
+        self.horshoe_points = pd.concat([Pcrp1.to_frame().transpose(),Pcrp2.to_frame().transpose(),Pcrp3.to_frame().transpose(),Pcrp4.to_frame().transpose()], sort=True).sort_index()
+
+        # Smoothing these points
+        tmp_id=0
+        self.org_triplet = copy.copy(self.triplet)
+        while tmp_id <= (len(self.horshoe_points) - 3):
+            self.triplet = self.horshoe_points.iloc[tmp_id:tmp_id+3]
+            self._crossing_point_optimisation()
+            _,_ = self._checking_crossing()
+            if not self._trigger_horeshoe:
+                self.horshoe_points.iloc[tmp_id:tmp_id+3] = self.triplet
+            else:
+                if abs(self.triplet.iloc[1]['case']) == 2:
+                    self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],self._vmin+1e-9,self._vmax-1e-9)
+                if abs(self.triplet.iloc[1]['case']) == 4:
+                    self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],self._vmin+1e-9,self._vmax-1e-9)  
+                self.horshoe_points.iloc[tmp_id:tmp_id+3] = self.triplet  
+            tmp_id+=1
+        self.triplet = copy.copy(self.org_triplet)
+        self._corner_created = True
+        return
 
-        self.CrossingDF = pd.concat([self.CrossingDF,newP.to_frame().transpose()]).sort_index().reset_index(drop=True) #self.CrossingDF.append(newP,sort=True).sort_index().reset_index(drop=True)
-        self.CrossingDF.index = np.arange(int(self.CrossingDF.index.min()),int(self.CrossingDF.index.max()*1e3 + 1e3),int(1e3))
 
 
-    def _mergePoint(self):
+    def _mergePoint(self,merge_distance = 1e-4):
         '''
-            FILL
+            Merging two points into a corner case if their distance is small enough.
         '''
+
         def PtDist(Ser1,Ser2):
             #return np.sqrt(self._calXDist(Ser2['cx'],Ser1['cx'])**2 + self._calXDist(Ser2['cy'],Ser1['cy'])**2)
             return np.sqrt((Ser1['cx'] - Ser2['cx'])**2 + (Ser1['cy'] - Ser2['cy'])**2)
 
         id=0
         while id < len(self.CrossingDF)-3:
             triplet = self.CrossingDF.iloc[id:id+3]
-            if PtDist(triplet.iloc[0],triplet.iloc[1]) < 2e-3:
+            if PtDist(triplet.iloc[0],triplet.iloc[1]) < merge_distance:
                 try:
                     neighbourIndex = np.where(np.array(triplet.iloc[0]['cellStart']['neighbourIndex'])==triplet.iloc[1]['cellEnd'].name)[0][0]
                 except:
                     id+=1
                     continue
                 case           = triplet['cellStart'].iloc[0]['case'][neighbourIndex]
                 crossingPoint  = triplet['cellStart'].iloc[0]['neighbourCrossingPoints'][neighbourIndex]
                 triplet['cx'].iloc[0]      = crossingPoint[0]
                 triplet['cy'].iloc[0]      = crossingPoint[1]
                 triplet['cellEnd'].iloc[0] = copy.deepcopy(triplet.iloc[1]['cellEnd'])
                 triplet['case'].iloc[0]    = copy.deepcopy(case)
                 self.CrossingDF           = self.CrossingDF.drop(triplet.iloc[1].name)
-            if PtDist(triplet.iloc[1],triplet.iloc[2]) < 2e-3:
+            if PtDist(triplet.iloc[1],triplet.iloc[2]) < merge_distance:
                 try:
                     neighbourIndex = np.where(np.array(triplet.iloc[1]['cellStart']['neighbourIndex'])==triplet.iloc[2]['cellEnd'].name)[0][0]
                 except:
                     id+=1
                     continue
                 case           = triplet['cellStart'].iloc[1]['case'][neighbourIndex]
                 crossingPoint  = triplet['cellStart'].iloc[1]['neighbourCrossingPoints'][neighbourIndex]
@@ -758,87 +1070,113 @@
                 triplet['cellEnd'].iloc[1] = copy.deepcopy(triplet.iloc[2]['cellEnd'])
                 triplet['case'].iloc[1]    = copy.deepcopy(case)
                 self.CrossingDF           = self.CrossingDF.drop(triplet.iloc[2].name)
 
             id+=1
 
         self.CrossingDF = self.CrossingDF.sort_index().reset_index(drop=True)
-        self.CrossingDF.index = np.arange(int(self.CrossingDF.index.min()),int(self.CrossingDF.index.max()*1e3 + 1e3),int(1e3))
 
 
+        # def PointDistance(CrossingDF):
+        #     dist = (np.array(CrossingDF['cx'])[1:]-np.array(CrossingDF['cx'])[:-1]) +(np.array(CrossingDF['cy'])[1:]-np.array(CrossingDF['cy'])[:-1])
+        #     return dist
+        # idx_merg_points = (PointDistance(self.CrossingDF) < merge_distance)
+        # while idx_merg_points.any():
+        #     idx = np.where(idx_merg_points)[0][0]
+        #     cellStart = self.CrossingDF.iloc[idx]['cellStart']
+        #     cellEnd   = self.CrossingDF.iloc[idx+1]['cellEnd']
+        #     neighbour_indx = np.where(cellStart['neighbourIndex']==cellEnd.name)[0][0]
+        #     self.CrossingDF.iloc[idx]['cellEnd'] = cellEnd
+        #     self.CrossingDF.iloc[idx]['case'] = cellStart['case'][neighbour_indx]
+        #     self.CrossingDF.iloc[idx]['cx']   = cellStart['neighbourCrossingPoints'][neighbour_indx][0]
+        #     self.CrossingDF.iloc[idx]['cy']   = cellStart['neighbourCrossingPoints'][neighbour_indx][1]
+        #     self.CrossingDF = self.CrossingDF.drop(self.CrossingDF.index[idx+1])
+        #     self.CrossingDF = self.CrossingDF.sort_index().reset_index(drop=True)
+        #     self.CrossingDF.index = np.arange(int(self.CrossingDF.index.min()),int(self.CrossingDF.index.max()*1e3 + 1e3),int(1e3))
+        #     idx_merg_points = (PointDistance(self.CrossingDF) < merge_distance)
 
-    def _horseshoe(self):
+        
+
+
+
+    def _checking_crossing(self):
         '''
-            FILL
+            Checks to determine if the crossing point has moved outside the domain.
         '''
-        # Defining the case information
+
+        self._trigger_horeshoe = False
         Cp             = tuple(self.triplet[['cx','cy']].iloc[1])
-        Sp             = tuple(self.triplet.iloc[0][['cx','cy']])
-        Np             = tuple(self.triplet.iloc[2][['cx','cy']])
-        
         cellStartGraph = self.triplet.iloc[1]['cellStart']
         cellEndGraph   = self.triplet.iloc[1]['cellEnd']        
-        case           = self.triplet['case'].iloc[1]
+        case           = self.triplet['case'].iloc[1]        
+
+        orgtriplet = copy.copy(self.triplet)
 
         # Returning if corner horseshoe case type
-        if abs(case)==1 or abs(case)==3 or abs(case)==0: 
-            return
+        if abs(case)==1 or abs(case)==3 or abs(case)==0:
+            # self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],cellStartGraph['cx']-cellStartGraph['dcx'] ,cellStartGraph['cx']+cellStartGraph['dcx']) 
+            # self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],cellStartGraph['cy']-cellStartGraph['dcy'] ,cellStartGraph['cy']+cellStartGraph['dcy']) 
+            return None,None
         elif abs(case) == 2:
             # Defining the min and max of the start and end cells
             smin = cellStartGraph['cy']-cellStartGraph['dcy'] 
             smax = cellStartGraph['cy']+cellStartGraph['dcy']
             emin = cellEndGraph['cy']-cellEndGraph['dcy']
             emax = cellEndGraph['cy']+cellEndGraph['dcy']
 
             # Defining the global min and max
             vmin = np.max([smin,emin])
             vmax = np.min([smax,emax])
 
             # Point crossingpoint on boundary between the two origional cells
-            if (Cp[1] > vmin) and (Cp[1] < vmax):
-                return
+            if (Cp[1] >= vmin) and (Cp[1] <= vmax):
+                self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],vmin+1e-9,vmax-1e-9)       
+                return None,None
 
             # If Start and end cells share a edge for the horesshoe 
-            if (Cp[1]<=smin) and (smin==emin):
+            if (Cp[1]<smin) and (smin==emin):
                 hrshCaseStart = 4
                 hrshCaseEnd   = 4
-            if (Cp[1]>=smax) and (smax==emax):
+            if (Cp[1]>smax) and (smax==emax):
                 hrshCaseStart = -4
                 hrshCaseEnd   = -4
 
             # --- Cases where StartCell is Larger than end Cell ---
-            if (Cp[1]>=emax) and (smax>emax):
+            if (Cp[1]>emax) and (smax>emax):
                 hrshCaseStart = case
                 hrshCaseEnd   = (-4)                
-            if (Cp[1]<=emin) and (smin<emin):
+            if (Cp[1]<emin) and (smin<emin):
                 hrshCaseStart = case
                 hrshCaseEnd   = (4)                   
 
             # --- Cases where StartCell is smaller than end Cell ---
-            if (Cp[1]>=smax) and (smax<emax):
+            if (Cp[1]>smax) and (smax<emax):
                 hrshCaseStart = -4
                 hrshCaseEnd   = -case
-            if (Cp[1]<=smin) and (emin<smin):
+            if (Cp[1]<smin) and (emin<smin):
                 hrshCaseStart = 4
-                hrshCaseEnd   = -case                    
+                hrshCaseEnd   = -case      
+
+            self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],vmin+1e-9,vmax-1e-9)               
 
         elif abs(case) == 4:
             # Defining the min and max of the start and end cells
             smin = cellStartGraph['cx']-cellStartGraph['dcx']
             smax = cellStartGraph['cx']+cellStartGraph['dcx']
             emin = cellEndGraph['cx']-cellEndGraph['dcx']
             emax = cellEndGraph['cx']+cellEndGraph['dcx']
 
             # Defining the global min and max
             vmin = np.max([smin,emin])
             vmax = np.min([smax,emax])
 
             # Point crossingpoint on boundary between the two origional cells
             if (Cp[0] >= vmin) and (Cp[0] <= vmax):
-                return
+                self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],vmin+1e-9,vmax-1e-9)  
+                return None,None
 
             # If Start and end cells share a edge for the horesshoe 
             if (Cp[0]<smin) and (smin==emin):
                 hrshCaseStart = -2
                 hrshCaseEnd   = -2
             if (Cp[0]>smax) and (smax==emax):
                 hrshCaseStart = 2
@@ -856,168 +1194,194 @@
             if (Cp[0]>smax) and (smax<emax):
                 hrshCaseStart = (2)
                 hrshCaseEnd   = -case
             if (Cp[0]<smin) and (emin<smin):
                 hrshCaseStart = (-2)
                 hrshCaseEnd   = -case   
 
+            self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],vmin+1e-9,vmax-1e-9)        
+            
+
+        if ('hrshCaseStart' in locals()) and ('hrshCaseEnd' in locals()):
+            return hrshCaseStart,hrshCaseEnd
+        else:
+            print(orgtriplet)
+            print(self.triplet)
+            raise Exception ('Issues')
+            return None,None
+
+
+
+    def _horseshoe(self):
+        '''
+            Introduces a horeshoe type in the path smoothing updating inbuilt horeshoe values.
+        '''
+        # Defining the case information
+        Cp             = tuple(self.triplet[['cx','cy']].iloc[1])
+        cellStartGraph = self.triplet.iloc[1]['cellStart']
+        cellEndGraph   = self.triplet.iloc[1]['cellEnd']        
+        case           = self.triplet['case'].iloc[1]
+        self._horseshoe_created = False
+
+        # Defining if horseshoe is created
+        hrshCaseStart,hrshCaseEnd = self._checking_crossing()
+
+        # If not creating a horeshoe return
+        if (type(hrshCaseStart) == type(None)) or (type(hrshCaseEnd) == type(None)):
+            return
 
         # Determining the neighbours of the start and end cells that are the horseshoe case
         startGraphNeighbours = [cellStartGraph['neighbourIndex'][ii] for ii in list(np.where(np.array(cellStartGraph['case'])==hrshCaseStart)[0])]
         endGraphNeighbours   = [cellEndGraph['neighbourIndex'][ii] for ii in list(np.where(np.array(cellEndGraph['case'])==hrshCaseEnd)[0])]
 
-        # If there is no neighbour trim back to the edge of the cell
-        if (len(startGraphNeighbours)==0) or (len(endGraphNeighbours)==0):
-            if abs(case) == 2:
-                self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],vmin,vmax)
-            if abs(case) == 4:
-                self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],vmin,vmax)        
-            return
 
-        
+        # -- Addition of two cellboxes in horeshoe construction
         if abs(hrshCaseStart) == abs(hrshCaseEnd):
             for sGN in startGraphNeighbours:
                 for eGN in endGraphNeighbours:
                     if (np.array(self.neighbour_graph.loc[sGN,'neighbourIndex'])==eGN).any() and (np.array(self.neighbour_graph.loc[eGN,'neighbourIndex'])==sGN).any():
+
+                        # Determining the additional cellbox information to add
                         sGNGraph = self.neighbour_graph.loc[sGN]
                         eGNGraph = self.neighbour_graph.loc[eGN]
 
-
                         try:
-
                             Crp1 = np.array(cellStartGraph['neighbourCrossingPoints'])[np.where(np.array(cellStartGraph['neighbourIndex']) == sGN)[0][0],:]
                             Crp2 = np.array(sGNGraph['neighbourCrossingPoints'])[np.where(np.array(sGNGraph['neighbourIndex']) == eGN)[0][0],:]
                             Crp3 = np.array(eGNGraph['neighbourCrossingPoints'])[np.where(np.array(eGNGraph['neighbourIndex']) == cellEndGraph.name)[0][0],:]
-                        
-                        except:
-                            if abs(case) == 2:
-                                self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],vmin,vmax)
-                            if abs(case) == 4:
-                                self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],vmin,vmax)        
+                        except:      
                             return
 
-                        # Trimminng back if the cell is worse off
-                        if ('SIC' in sGNGraph) and ('SIC' in cellStartGraph) and (sGNGraph['SIC'] - cellStartGraph['SIC'])>=2:
-                            if abs(case) == 2:
-                                self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],vmin,vmax)
-                            if abs(case) == 4:
-                                self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],vmin,vmax)        
-                            return
-
-
-                        # Trimminng back if the cell is worse off fuel
-                        if ('fuel' in sGNGraph) and ('fuel' in cellStartGraph) and (sGNGraph['fuel'] - cellStartGraph['fuel'])>=2:
-                            if abs(case) == 2:
-                                self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],vmin,vmax)
-                            if abs(case) == 4:
-                                self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],vmin,vmax)        
-                            return
-
-
-                        # Updating the origional crossing point
-                        self.triplet['cx'].iloc[1]      = Crp1[0]
-                        self.triplet['cy'].iloc[1]      = Crp1[1]
-                        self.triplet['cellEnd'].iloc[1] = copy.deepcopy(sGNGraph)
-                        self.triplet['case'].iloc[1]    = self.triplet['cellStart'].iloc[1]['case'][np.where(np.array(self.triplet['cellStart'].iloc[1]['neighbourIndex'])==sGNGraph.name)[0][0]]
+                        # Crossing Point 1
+                        Pcrp1 = copy.deepcopy(self.triplet.iloc[0])
 
                         # Crossing Point 2
                         Pcrp2 = pd.Series(name=self.triplet.iloc[1].name+1,dtype='object')
-                        Pcrp2['cx']        = Crp2[0]
-                        Pcrp2['cy']        = Crp2[1]
-                        Pcrp2['cellStart'] = copy.deepcopy(sGNGraph)
-                        Pcrp2['cellEnd']   = copy.deepcopy(eGNGraph)
-                        Pcrp2['case']      = Pcrp2['cellStart']['case'][np.where(np.array(Pcrp2['cellStart']['neighbourIndex'])==Pcrp2['cellEnd'].name)[0][0]]
-
+                        Pcrp2['cx']        = Crp1[0]
+                        Pcrp2['cy']        = Crp1[1]
+                        Pcrp2['cellStart'] = copy.deepcopy(self.triplet['cellStart'].iloc[1])
+                        Pcrp2['cellEnd']   = copy.deepcopy(sGNGraph)
+                        Pcrp2['case']      = hrshCaseStart
+                        # Crossing Point 3
                         Pcrp3 = pd.Series(name=self.triplet.iloc[1].name+2,dtype='object')
-                        Pcrp3['cx']        = Crp3[0]
-                        Pcrp3['cy']        = Crp3[1]
-                        Pcrp3['cellStart'] = copy.deepcopy(eGNGraph)
-                        Pcrp3['cellEnd']   = copy.deepcopy(cellEndGraph)
-                        Pcrp3['case']      = Pcrp3['cellStart']['case'][np.where(np.array(Pcrp3['cellStart']['neighbourIndex'])==Pcrp3['cellEnd'].name)[0][0]]
+                        Pcrp3['cx']        = Crp2[0]
+                        Pcrp3['cy']        = Crp2[1]
+                        Pcrp3['cellStart'] = copy.deepcopy(sGNGraph)
+                        Pcrp3['cellEnd']   = copy.deepcopy(eGNGraph)
+                        Pcrp3['case']      = case
+                        # Crossing Point 4
+                        Pcrp4 = pd.Series(name=self.triplet.iloc[1].name+3,dtype='object')
+                        Pcrp4['cx']        = Crp3[0]
+                        Pcrp4['cy']        = Crp3[1]
+                        Pcrp4['cellStart'] = copy.deepcopy(eGNGraph)
+                        Pcrp4['cellEnd']   = copy.deepcopy(cellEndGraph)
+                        Pcrp4['case']      = -hrshCaseEnd
+
+                        Pcrp5 = copy.deepcopy(self.triplet.iloc[2])
+
+                        self.horshoe_points = pd.concat([Pcrp1.to_frame().transpose(),Pcrp2.to_frame().transpose(),Pcrp3.to_frame().transpose(),Pcrp4.to_frame().transpose(),Pcrp5.to_frame().transpose()], sort=True).sort_index()
+
+                        # Smoothing these points
+                        tmp_id=0
+                        self.org_triplet = copy.copy(self.triplet)
+                        while tmp_id <= (len(self.horshoe_points) - 3):
+                            self.triplet = self.horshoe_points.iloc[tmp_id:tmp_id+3]
+                            self._crossing_point_optimisation()
+                            _,_ = self._checking_crossing()
+                            if not self._trigger_horeshoe:
+                                self.horshoe_points.iloc[tmp_id:tmp_id+3] = self.triplet
+                            else:
+                                if abs(self.triplet.iloc[1]['case']) == 2:
+                                    self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],self._vmin+1e-9,self._vmax-1e-9)
+                                if abs(self.triplet.iloc[1]['case']) == 4:
+                                    self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],self._vmin+1e-9,self._vmax-1e-9)  
+                                self.horshoe_points.iloc[tmp_id:tmp_id+3] = self.triplet  
+                            tmp_id+=1
+                        self.triplet = copy.copy(self.org_triplet)
                         
-
-                        self.CrossingDF = pd.concat([self.CrossingDF,Pcrp2.to_frame().transpose(),Pcrp3.to_frame().transpose()], sort=True).sort_index().reset_index(drop=True) #self.CrossingDF.append([Pcrp2,Pcrp3],sort=True).sort_index().reset_index(drop=True)
-
-                        self.CrossingDF.index = np.arange(int(self.CrossingDF.index.min()),int(self.CrossingDF.index.max()*1e3 + 1e3),int(1e3))
-
-                        break
-
-            if abs(case) == 2:
-                self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],vmin,vmax)
-            if abs(case) == 4:
-                self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],vmin,vmax)        
-            return
-        else:
+                        
+                        self._horseshoe_created = True
+                        break       
+        
+        # -- Addition of one cellboxes in horeshoe construction, corner adddition
+        if abs(hrshCaseStart) != abs(hrshCaseEnd):
             for sGN in startGraphNeighbours:
                 for eGN in endGraphNeighbours:
                     if (np.array(sGN==eGN).any()):
-                        
                         NeighGraph = self.neighbour_graph.loc[sGN]            
-                        
-                        
                         try:
                             Crp1 = np.array(cellStartGraph['neighbourCrossingPoints'])[np.where(np.array(cellStartGraph['neighbourIndex']) == sGN)[0][0],:]
                             Crp2 = np.array(NeighGraph['neighbourCrossingPoints'])[np.where(np.array(NeighGraph['neighbourIndex']) == cellEndGraph.name)[0][0],:]
-
-                        except:
-                            if abs(case) == 2:
-                                self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],vmin,vmax)
-                            if abs(case) == 4:
-                                self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],vmin,vmax)        
-                            return
-
-
-                        # Trimminng back if the cell is worse off
-                        if ('SIC' in NeighGraph) and ('SIC' in cellStartGraph) and (NeighGraph['SIC'] - cellStartGraph['SIC'])>=2:
-                            if abs(case) == 2:
-                                self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],vmin,vmax)
-                            if abs(case) == 4:
-                                self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],vmin,vmax)        
-                            return
-
-                        # Trimminng back if the cell is worse off fuel
-                        if ('fuel' in NeighGraph) and ('fuel' in cellStartGraph) and (NeighGraph['fuel'] - cellStartGraph['fuel'])>=2:
-                            if abs(case) == 2:
-                                self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],vmin,vmax)
-                            if abs(case) == 4:
-                                self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],vmin,vmax)        
+                        except: 
                             return
 
 
+                        # Crossing point 1
+                        Pcrp1 = copy.deepcopy(self.triplet.iloc[0])
+                        # Crossing point 2
+                        Pcrp2 = pd.Series(name=self.triplet.iloc[1].name+1,dtype='object')
+                        Pcrp2['cx']        = Crp1[0]
+                        Pcrp2['cy']        = Crp1[1]
+                        Pcrp2['cellStart'] = copy.deepcopy(self.triplet['cellStart'].iloc[1])
+                        Pcrp2['cellEnd']   = copy.deepcopy(NeighGraph)
+                        Pcrp2['case']      = hrshCaseStart
+                        # Crossing point 3
+                        Pcrp3 = pd.Series(name=self.triplet.iloc[1].name+2,dtype='object')
+                        Pcrp3['cx']        = Crp2[0]
+                        Pcrp3['cy']        = Crp2[1]
+                        Pcrp3['cellStart'] = copy.deepcopy(NeighGraph)
+                        Pcrp3['cellEnd']   = copy.deepcopy(cellEndGraph)
+                        Pcrp3['case']      = -hrshCaseEnd
+                        # Crossing point 4
+                        Pcrp4 = copy.deepcopy(self.triplet.iloc[2])
+            
+                        self.horshoe_points = pd.concat([Pcrp1.to_frame().transpose(),Pcrp2.to_frame().transpose(),Pcrp3.to_frame().transpose(),Pcrp4.to_frame().transpose()], sort=True).sort_index()
+
+                        # Smoothing these points
+                        self.org_triplet = copy.copy(self.triplet)
+                        tmp_id=0
+                        while tmp_id <= (len(self.horshoe_points) - 3):
+                            self.triplet = self.horshoe_points.iloc[tmp_id:tmp_id+3]
+                            self._crossing_point_optimisation()
+                            _,_ = self._checking_crossing()
+                            if not self._trigger_horeshoe:
+                                self.horshoe_points.iloc[tmp_id:tmp_id+3] = self.triplet
+                            else:
+                                if abs(self.triplet.iloc[1]['case']) == 2:
+                                    self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],self._vmin+1e-9,self._vmax-1e-9)
+                                if abs(self.triplet.iloc[1]['case']) == 4:
+                                    self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],self._vmin+1e-9,self._vmax-1e-9)  
+                                self.horshoe_points.iloc[tmp_id:tmp_id+3] = self.triplet  
+                            tmp_id+=1    
 
-                        # Updating the origional crossing point
-                        self.triplet['cx'].iloc[1]      = Crp1[0]
-                        self.triplet['cy'].iloc[1]      = Crp1[1]
-                        self.triplet['cellEnd'].iloc[1] = copy.deepcopy(NeighGraph)
-                        self.triplet['case'].iloc[1]    = self.triplet['cellStart'].iloc[1]['case'][np.where(np.array(self.triplet['cellStart'].iloc[1]['neighbourIndex'])==NeighGraph.name)[0][0]]
-
-                        Pcrp2 = pd.Series(name=self.triplet.iloc[1].name+2,dtype='object')
-                        Pcrp2['cx']        = Crp2[0]
-                        Pcrp2['cy']        = Crp2[1]
-                        Pcrp2['cellStart'] = copy.deepcopy(NeighGraph)
-                        Pcrp2['cellEnd']   = copy.deepcopy(cellEndGraph)
-                        Pcrp2['case']      = Pcrp2['cellStart']['case'][np.where(np.array(Pcrp2['cellStart']['neighbourIndex'])==Pcrp2['cellEnd'].name)[0][0]]
-                        
-                        self.CrossingDF = pd.concat([self.CrossingDF,Pcrp2.to_frame().transpose()], sort=True).sort_index().reset_index(drop=True)#self.CrossingDF.append([Pcrp2],sort=True).sort_index().reset_index(drop=True)
-                        
-                        self.CrossingDF.index = np.arange(int(self.CrossingDF.index.min()),int(self.CrossingDF.index.max()*1e3 + 1e3),int(1e3))
+                        self.triplet = copy.copy(self.org_triplet)
 
+                        self._horseshoe_created = True
                         break
 
-            if abs(case) == 2:
-                self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],vmin,vmax)
-            if abs(case) == 4:
-                self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],vmin,vmax)        
-            return
+        # if abs(case) == 2:
+        #     self.triplet['cy'].iloc[1] = np.clip(self.triplet.iloc[1]['cy'],vmin+1e-9,vmax-1e-9)
+        # if abs(case) == 4:
+        #     self.triplet['cx'].iloc[1] = np.clip(self.triplet.iloc[1]['cx'],vmin+1e-9,vmax-1e-9)        
+        # return
                 
 
     def _reverseCase(self):
         '''
             FILL
         '''
+
+        # ====== Finding Reverse Edges ======
+
+
+
+
+        # ====== Correcting Cases Over Points =====
+
+
         # Removing Reverse Edge Type 1
         startIndex = np.array([row['cellStart'].name for idx,row in self.CrossingDF.iterrows()][1:-1])
         endIndex   = np.array([row['cellEnd'].name for idx,row in self.CrossingDF.iterrows()][1:-1] )
         boolReverseEdge  = np.logical_and((startIndex[:-1] == endIndex[1:]),(startIndex[1:] == endIndex[:-1]))
         if boolReverseEdge.any():
             indxReverseEdge = np.where(boolReverseEdge)[0]+1
             for id in indxReverseEdge:
@@ -1043,97 +1407,70 @@
                 self.CrossingDF = self.CrossingDF.drop(self.CrossingDF.iloc[id].name).sort_index().reset_index(drop=True)
 
 
 
         self.CrossingDF.index = np.arange(0,int(len(self.CrossingDF)*1e3),int(1e3))
 
 
-    def _updateCrossingPoint(self):
-        '''
-            FILL
-        '''
-
-        self.org_triplet = copy.deepcopy(self.triplet) 
-        self.speed_s = self._unit_speed(self.triplet.iloc[1]['cellStart']['Speed'])
-        self.speed_e = self._unit_speed(self.triplet.iloc[1]['cellEnd']['Speed'])
+    def _crossing_point_optimisation(self):
+        self._corner_created = False
 
-        # ------ Case Deginitions & Dealing
+        # ------ Case Definitions & Dealing
         if self.debugging:
             print('===========================================================')
         if abs(self.triplet.iloc[1].case)==2:
             self._long_case()
         elif abs(self.triplet.iloc[1].case)==4:
             self._lat_case()
         elif (abs(self.triplet.iloc[1].case)==1) or (abs(self.triplet.iloc[1].case)==3):
             self._corner_case()
+        # Determining if crossing point lies outside of interface between two cellboxes
+        
 
-        if len(self.triplet) < 3:
-            return
+    def _updateCrossingPoint(self,iter):
 
+        self.org_points = copy.deepcopy(self.triplet)
 
+        case = self.triplet.iloc[1].case
+        indx = np.where(self.indx_type==case)[0][0]
 
+        self.speed_s = self._unit_speed(copy.copy(self.triplet.iloc[1]['cellStart']['speed'][indx]))
+        self.speed_e = self._unit_speed(copy.copy(self.triplet.iloc[1]['cellEnd']['speed'][indx]))
 
-    def _traveltime_in_cell(self,xdist,ydist,U,V,S):
-        '''
-            FILL
-        '''
-        dist  = np.sqrt(xdist**2 + ydist**2)
-        cval  = np.sqrt(U**2 + V**2)
+        # --- Updating the crossing point
+        self._crossing_point_optimisation()
 
-        dotprod  = xdist*U + ydist*V
-        diffsqrs = S**2 - cval**2
+        # --- Additional Cells & Reverse Edges
+        self._horseshoe()
 
-        # if (dotprod**2 + diffsqrs*(dist**2) < 0)
-        if diffsqrs == 0.0:
-            if dotprod == 0.0:
-                return np.inf
-                #raise Exception(' ')
-            else:
-                if ((dist**2)/(2*dotprod))  <0:
-                    return np.inf
-                    #raise Exception(' ')
-                else:
-                    traveltime = dist * dist / (2 * dotprod)
-                    return traveltime
+        if (self._horseshoe_created == True) or (self._corner_created==True):
+            org_variables = self.objective_function(self.org_points)
+            new_variables = self.objective_function(self.horshoe_points)
 
-        traveltime = (np.sqrt(dotprod**2 + (dist**2)*diffsqrs) - dotprod)/diffsqrs
-        if traveltime < 0:
-            traveltime = np.inf
-        return traveltime, dist
+            self._horshoe_percentage_improvement = ((new_variables[self.objective_func]['path_values'][-1] - org_variables[self.objective_func]['path_values'][-1])/org_variables[self.objective_func]['path_values'][-1])*100
 
-    def _waypoint_correction(self,source_graph,Wp,Cp):
-        '''
-            FILL
-        '''
-        m_long  = 111.321*1000
-        m_lat   = 111.386*1000
+            if  self._horshoe_percentage_improvement > -10:
+                horeshoe_points     = self.horshoe_points[['cx','cy']].iloc[1:-1].to_numpy()
+                same_horseshoes_num = count_similarities(horeshoe_points.tolist(),self.previous_horeshoes)
+                if same_horseshoes_num <=3:
+                    self.CrossingDF = self.CrossingDF.drop(self.triplet.index)
+                    self.CrossingDF = pd.concat([self.CrossingDF, self.horshoe_points]).sort_index().reset_index(drop=True)
+                    self.previous_horeshoes += [[iter,self.horshoe_points[['cx','cy']].iloc[1:-1].to_numpy().tolist(),self._horshoe_percentage_improvement]]
 
-        x = (Cp[0]-Wp[0])*m_long*np.cos(Wp[1]*(np.pi/180))
-        y = (Cp[1]-Wp[1])*m_lat
-        Su  = source_graph['Vector_x']*self.zc
-        Sv  = source_graph['Vector_y']*self.zc
-        Ssp = self._unit_speed(source_graph['Speed'])
-        traveltime, distance = self._traveltime_in_cell(x,y,Su,Sv,Ssp)
-        return traveltime, distance
+        self._reverseCase()
+        self.CrossingDF = self.CrossingDF.reset_index(drop=True)
+        self.CrossingDF.index = np.arange(int(self.CrossingDF.index.min()),int(self.CrossingDF.index.max()*1e3 + 1e3),int(1e3))
 
-    def objective_function(self):
-        '''
-            FILL
-        '''
-        TravelTime = np.zeros(len(self.CrossingDF))
-        Distance   = np.zeros(len(self.CrossingDF))
-        index      = np.zeros(len(self.CrossingDF))
-        for ii in range(len(self.CrossingDF)-1):
-            soruce_graph = self.CrossingDF.iloc[ii]['cellEnd']
-            Wp = self.CrossingDF.iloc[ii][['cx','cy']].to_numpy()
-            Cp = self.CrossingDF.iloc[ii+1][['cx','cy']].to_numpy()
-            traveltime, distance = self._waypoint_correction(soruce_graph,Wp,Cp)
-            TravelTime[ii+1] = self._unit_time(traveltime)
-            Distance[ii+1]   = distance
-
-            if ii ==0:
-                index[ii] = soruce_graph.name
-                index[ii+1] = soruce_graph.name
-            else:
-                index[ii+1] = soruce_graph.name
-        return TravelTime,Distance,index
 
+
+def count_similarities(horshoe_points,previous_horeshoes):
+    comparison = []
+    if len(previous_horeshoes) == 0:
+        return 0
+    for entry in previous_horeshoes:
+        old_horeshoes = entry[1]
+        similar = (horshoe_points == old_horeshoes)
+        if type(similar) == bool:
+            comparison += [similar]
+        else:
+            comparison += [similar.all()]
+    return len(np.where(comparison)[0])
```

### Comparing `polar_route-0.0.15/polar_route/route_planner.py` & `polar_route-0.1.0/polar_route/route_planner.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,14 +25,43 @@
     for case in neighbours.keys():
         for neighbour in neighbours[case]:
             neighbour_case.append(int(case))
             neighbour_indx.append(int(neighbour))
     return neighbour_case, neighbour_indx
 
 
+
+
+def _json_str(input):
+    if type(input) is dict:
+        output = input
+    elif type(input) is str:
+        try:
+            with open(input, 'r') as f:
+                output = json.load(f)
+        except:
+            raise Exception("Unable to load '{}', please check path name".format(input))
+    return output
+
+def _pandas_dataframe_str(input):
+    if type(input) is dict:
+        output = input
+    elif type(input) == type(pd.DataFrame()):
+        output = input
+    elif type(input) is str:
+        try:
+            output = pd.read_csv(input)
+        except:
+            raise Exception("Unable to load '{}', please check path name".format(input))
+    return output
+
+
+
+
+
 class RoutePlanner:
     """
         ---
 
         RoutePlanner optimises the route paths between a series of waypoints. 
         The routes are constructed in a two stage process:
 
@@ -103,60 +132,59 @@
                     ]}\n
                 }\n
 
         ---
 
     """
 
-    def __init__(self, mesh, waypoints, cost_func=NewtonianDistance):
+    def __init__(self, mesh, config, waypoints, cost_func=NewtonianDistance):
 
         """
             Constructs the routes from information given in the config file.
 
             Args:
-                config (dict): config file which defines the attributes required for the route construction. 
+
+                mesh(dict or string of filepath): mesh based JSON containing the cellbox information and neighbourhood graph
+
+                config (dict or string of filepath): config JSON which defines the attributes required for the route construction. 
                     Sections required for the route construction are as follows\n
                     \n
                     {\n
-                        "config": {...\n
-                            "Route_Info":{\n
-                                    "objective_function": (string) currently either 'traveltime' or 'fuel',\n
-                                    "path_variables": list of (string),\n
-                                    "waypoints_path": (string),\n
-                                    "source_waypoints": list of (string),\n
-                                    "end_waypoints": list of (string),\n
-                                    "vector_names": (list of (string),\n
-                                    "zero_currents": (boolean),\n
-                                    "variable_speed" (boolean),\n
-                                    "time_unit" (string),\n
-                                    "early_stopping_criterion" (boolean),\n
-                                    "save_dijkstra_graphs": (boolean),\n
-                                    "smooth_path":{\n
-                                        "max_iteration_number":(int),\n
-                                        "minimum_difference":(float),\n
-                                    }\n
-                                },\n
-                        }\n
+                        "objective_function": (string) currently either 'traveltime' or 'fuel',\n
+                        "path_variables": list of (string),\n
+                        "waypoints_path": (string),\n
+                        "source_waypoints": list of (string),\n
+                        "end_waypoints": list of (string),\n
+                        "vector_names": (list of (string),\n
+                        "zero_currents": (boolean),\n
+                        "variable_speed" (boolean),\n
+                        "time_unit" (string),\n
+                        "early_stopping_criterion" (boolean),\n
+                        "save_dijkstra_graphs": (boolean),\n
+                        "smooth_path":{\n
+                            "max_iteration_number":(int),\n
+                            "minimum_difference":(float),\n
                     }\n
 
                 cost_func (func): Crossing point cost function for Dijkstra Path creation. For development purposes only !
         """
 
         # Load in the current cell structure & Optimisation Info̦
-        # self.mesh    = copy.copy(mesh)
-        self.mesh = mesh
-        self.config  = self.mesh['config']
-
-        waypoints_df = pd.read_csv(waypoints)
+        self.mesh             = _json_str(mesh)
+        self.config           = _json_str(config)
+        waypoints_df          = _pandas_dataframe_str(waypoints)
         source_waypoints_df   = waypoints_df[waypoints_df['Source'] == "X"]
         des_waypoints_df      = waypoints_df[waypoints_df['Destination'] == "X"]
 
         self.source_waypoints = list(source_waypoints_df['Name'])
         self.end_waypoints    = list(des_waypoints_df['Name'])
 
+        # Case indices
+        self.indx_type = np.array([1, 2, 3, 4, -1, -2, -3, -4])
+
         # Creating a blank path construct
         self.paths          = None
         self.smoothed_paths = None
         self.dijkstra_info = {}
 
         # ====== Loading Mesh & Neighbour Graph ======
         # Formatting the Mesh and Neighbour Graph to the right form
@@ -169,63 +197,59 @@
 
         # Using neighbour graph to determine neighbour indices and cases
         self.neighbour_graph['case'], self.neighbour_graph['neighbourIndex'] = zip(*self.neighbour_graph.apply(lambda row: _flattenCases(row.name, self.mesh), axis=1))
 
         self.neighbour_graph.index = self.neighbour_graph.index.astype(int)
 
         # Renaming the vector columns
-        self.neighbour_graph = self.neighbour_graph.rename(columns={self.config['Route_Info']['vector_names'][0]: "Vector_x", 
-                                                                    self.config['Route_Info']['vector_names'][1]: "Vector_y"})
+        self.neighbour_graph = self.neighbour_graph.rename(columns={self.config['vector_names'][0]: "Vector_x", 
+                                                                    self.config['vector_names'][1]: "Vector_y"})
 
         # ====== Speed Function Checking ======
         # Checking if Speed defined in file
-        if 'Speed' not in self.neighbour_graph:
-            self.neighbour_graph['Speed'] = self.config["Vessel"]["Speed"]
+        if 'speed' not in self.neighbour_graph:
+            print(self.neighbour_graph.columns)
+            raise Exception('Vessel Speed not in the mesh information ! Please run vessel performance')
 
         # ====== Objective Function Information ======
         #  Checking if objective function is in the cellgrid            
-        if self.config['Route_Info']['objective_function'] != 'traveltime':
-            if self.config['Route_Info']['objective_function'] not in self.neighbour_graph:
-                raise Exception("Objective Function require '{}' column in mesh dataframe".format(self.config['Route_Info']['objective_function']))
+        if self.config['objective_function'] != 'traveltime':
+            if self.config['objective_function'] not in self.neighbour_graph:
+                raise Exception("Objective Function require '{}' column in mesh dataframe".format(self.config['objective_function']))
 
         # ===== Dijkstra Graph =====
         # Adding the required columns needed for the dijkstra graph
         self.neighbour_graph['positionLocked']          = False
-        for vrbl in self.config['Route_Info']['path_variables']:
+        for vrbl in self.config['path_variables']:
             self.neighbour_graph['shortest_{}'.format(vrbl)]    = np.inf
         self.neighbour_graph['neighbourTravelLegs']     = [list() for x in range(len(self.neighbour_graph.index))]
         self.neighbour_graph['neighbourCrossingPoints'] = [list() for x in range(len(self.neighbour_graph.index))]
         self.neighbour_graph['pathIndex']               = [list() for x in range(len(self.neighbour_graph.index))]
-        for vrbl in self.config['Route_Info']['path_variables']:
+        for vrbl in self.config['path_variables']:
             self.neighbour_graph['path_{}'.format(vrbl)] = [list() for x in range(len(self.neighbour_graph.index))]
         self.neighbour_graph['pathPoints']               = [list() for x in range(len(self.neighbour_graph.index))]
 
         # ====== Defining the cost function ======
         self.cost_func       = cost_func
 
         # ====== Outlining some constant values ======
-        self.unit_shipspeed = self.config['Vessel']['Unit']
-        self.unit_time      = self.config['Route_Info']['time_unit']
-        self.zero_currents  = self.config['Route_Info']['zero_currents']
-        self.variable_speed  =self.config['Route_Info']['variable_speed']
-
-        if not self.variable_speed:
-            self.neighbour_graph['Speed'] = self.config["Vessel"]["Speed"]
+        self.unit_time       = self.config['time_unit']
+        self.zero_currents   = self.config['zero_currents']
+        self.variable_speed  = self.config['variable_speed']
+        if type(self.variable_speed) == float:
+            logging.info(' Defining a constant speed map = {}'.format(self.variable_speed))
+            self.neighbour_graph['speed'] = self.variable_speed
+            cbxs = pd.DataFrame(self.mesh['cellboxes'])
+            cbxs['speed'] = self.variable_speed
+            self.mesh['cellboxes'] = cbxs.to_dict('records')
 
         # ====== Waypoints ======
         self.mesh['waypoints'] = waypoints_df
 
-        # Dropping waypoints outside domain
-        self.mesh['waypoints'] = self.mesh['waypoints'][\
-                                                              (self.mesh['waypoints']['Long'] >= self.config['Mesh_info']['Region']['longMin']) &\
-                                                              (self.mesh['waypoints']['Long'] <=  self.config['Mesh_info']['Region']['longMax']) &\
-                                                              (self.mesh['waypoints']['Lat'] <=  self.config['Mesh_info']['Region']['latMax']) &\
-                                                              (self.mesh['waypoints']['Lat'] >=  self.config['Mesh_info']['Region']['latMin'])] 
-
-        # # Initialising Waypoints positions and cell index
+        # Initialising Waypoints positions and cell index
         wpts = self.mesh['waypoints']
         wpts['index'] = np.nan
         for idx,wpt in wpts.iterrows():
             indices = self.neighbour_graph[self.neighbour_graph['geometry'].contains(Point(wpt[['Long','Lat']]))].index
             # Waypoint is not within a mesh cell, but could still be on the edge of one. So perturbing the position slightly to the north-east and checking again. 
             #If this is not the case then the waypoint is not within the navitagatable domain and will continue
             if len(indices) == 0:
@@ -243,36 +267,61 @@
         self.mesh['waypoints'] = wpts[~wpts['index'].isnull()]
         self.mesh['waypoints']['index'] = self.mesh['waypoints']['index'].astype(int)
         self.mesh['waypoints'] =  self.mesh['waypoints'].to_json()
 
         # ==== Printing Configuration and Information
         self.mesh['waypoints'] =  pd.read_json(self.mesh['waypoints'])
 
+        # # ===== Running the route planner for the given information
+        # if ("dijkstra_only" in self.config) and self.config['dijkstra_only']:
+        #     self.compute_routes()
+        # else:
+        #     self.compute_routes()
+        #     self.compute_smoothed_routes()
+
+
+        # # === Saving file to output or saving it to variable output
+        # output = self.to_json()
+        # if ('output' in self.config) and (type(self.config['output']) == str):
+        #     with open(self.config['output'], 'w') as f:
+        #         json.dump(output,f)
+        # else:
+        #     self.output = output
+
+
 
     def to_json(self):
         '''
             Outputing the information in JSON format
         '''
         mesh = copy.copy(self.mesh)
         mesh['waypoints'] = mesh['waypoints'].to_dict()
+        mesh['config']['route_info'] = self.config
         output_json = json.loads(json.dumps(mesh))
         del mesh
         return output_json
 
     def _dijkstra_paths(self, start_waypoints, end_waypoints):
         """
-            FILL
+            Hidden function. Given internal variables and start and end waypoints this function
+            returns a GEOJSON formated path dict object
+
+            INPUTS:
+                start_waypoints: Start waypoint names (list)
+                end_waypoints: End waypoint names (list)
         """
 
         geojson = dict()
         geojson['type'] = "FeatureCollection"
 
         paths = []
         wpts_s = self.mesh['waypoints'][self.mesh['waypoints']['Name'].isin(start_waypoints)]
         wpts_e = self.mesh['waypoints'][self.mesh['waypoints']['Name'].isin(end_waypoints)]
+
+
         for _, wpt_a in wpts_s.iterrows():
             wpt_a_name  = wpt_a['Name']
             wpt_a_index = int(wpt_a['index'])
             wpt_a_loc   = [[wpt_a['Long'],wpt_a['Lat']]]
             for _, wpt_b in wpts_e.iterrows():
                 wpt_b_name  = wpt_b['Name']
                 wpt_b_index = int(wpt_b['index'])
@@ -292,56 +341,86 @@
                         path['properties']['from'] = '{}'.format(wpt_a_name)
                         path['properties']['to'] = '{}'.format(wpt_b_name)
 
                         cellIndices  = np.array(graph['pathIndex'].loc[wpt_b_index])
                         path_indices = np.array([cellIndices[0]] + list(np.repeat(cellIndices[1:-1], 2)) + [cellIndices[-1]])
                         path['properties']['CellIndices'] = path_indices.tolist()
 
+                        cases = []
+
+                        # Determine cases for cell pairs along the path
+                        for idx in range(len(cellIndices) -1):
+                            cellStart = graph.loc[cellIndices[idx]]
+                            cellEnd = graph.loc[cellIndices[idx+1]]
+                            case = cellStart['case'][np.where(np.array(cellStart['neighbourIndex']) == cellEnd.name)[0][0]]
+                            cases+=[case]
+
+                        start_case = cases[0]
+                        end_case = cases[-1]
+
+                        # Full list of cases for each leg (centre to crossing point and crossing point to centre)
+                        path_cases = list(np.repeat(cases, 2))
+
                         # Applying in-cell correction for travel-time
                         cost_func    = self.cost_func(source_graph=self.dijkstra_info[wpt_a_name].loc[path_indices[0]],
                                                       neighbour_graph=self.dijkstra_info[wpt_a_name].loc[path_indices[0]],
-                                                      unit_shipspeed='km/hr', unit_time=self.unit_time, zerocurrents=self.zero_currents)
+                                                      unit_shipspeed='km/hr', unit_time=self.unit_time, zerocurrents=self.zero_currents,
+                                                      case=start_case)
                         tt_start = cost_func.waypoint_correction(path_points[0, :], path_points[1, :])
                         cost_func    = self.cost_func(source_graph=self.dijkstra_info[wpt_a_name].loc[path_indices[-1]],
                                                       neighbour_graph=self.dijkstra_info[wpt_a_name].loc[path_indices[0]],
-                                                      unit_shipspeed='km/hr', unit_time=self.unit_time, zerocurrents=self.zero_currents)
+                                                      unit_shipspeed='km/hr', unit_time=self.unit_time, zerocurrents=self.zero_currents,
+                                                      case=end_case)
+
                         tt_end = cost_func.waypoint_correction(path_points[-1, :], path_points[-2, :])
                         path['properties']['traveltime']     = np.array(graph['path_traveltime'].loc[wpt_b_index])
                         path['properties']['traveltime']     = (path['properties']['traveltime'] - path['properties']['traveltime'][0]) + tt_start
                         path['properties']['traveltime'][-1] = (path['properties']['traveltime'][-2] + tt_end)
+                        path['properties']['cases'] = [int(p) for p in path_cases]
 
-                        for vrbl in self.config['Route_Info']['path_variables']:
+                        for vrbl in self.config['path_variables']:
                             if vrbl == 'traveltime':
                                 continue
-                            path['properties'][vrbl] = np.cumsum(np.r_[path['properties']['traveltime'][0], np.diff(path['properties']['traveltime'])]*self.dijkstra_info[wpt_a_name].loc[path_indices,'{}'.format(vrbl)].to_numpy()).tolist()
+                            traveltime_diff = np.r_[path['properties']['traveltime'][0], np.diff(path['properties']['traveltime'])]
+                            variable_vals = graph.loc[path_indices, '{}'.format(vrbl)]
+                            case_vals = pd.Series(data=[v[np.where(self.indx_type==path_cases[i])[0][0]] for i, v in enumerate(variable_vals)],
+                                                  index=variable_vals.index)
+                            variable_diff = traveltime_diff*case_vals
+                            path['properties'][vrbl] = np.cumsum(variable_diff.to_numpy()).tolist()
                         path['properties']['traveltime'] = path['properties']['traveltime'].tolist()
                         paths.append(path)
 
                     except:
-                        logging.warning('{} to {} - Failured to construct path direct in the dijkstra information'.format(wpt_a_name,wpt_b_name))
+                        logging.warning('{} to {} - Failed to construct path direct in the dijkstra information'.format(wpt_a_name,wpt_b_name))
 
         geojson['features'] = paths
         return geojson
 
-    def _objective_value(self, variable, source_graph, neighbour_graph, traveltime):
+
+
+    def _objective_value(self, variable, source_graph, neighbour_graph, traveltime, case):
         """
-            FILL
+            Hidden variable. Returns the objective value between two cellboxes.
         """
         if variable == 'traveltime':
-            return np.array([source_graph['shortest_traveltime'] + traveltime[0],source_graph['shortest_traveltime'] + np.sum(traveltime)])
+            objs = np.array([source_graph['shortest_traveltime'] + traveltime[0],source_graph['shortest_traveltime'] + np.sum(traveltime)])
+            return objs
         else:
-            return np.array([source_graph['shortest_{}'.format(variable)] +\
-                    traveltime[0]*source_graph['{}'.format(variable)],
-                    source_graph['shortest_{}'.format(variable)] +\
-                    traveltime[0]*source_graph['{}'.format(variable)] +\
-                    traveltime[1]*neighbour_graph['{}'.format(variable)]])
+            if type(source_graph['{}'.format(variable)]) == list and len(source_graph['{}'.format(variable)]) != 1:
+                idx = np.where(self.indx_type==case)[0][0]
+                objs = np.array([source_graph['shortest_{}'.format(variable)] + traveltime[0]*source_graph['{}'.format(variable)][idx],source_graph['shortest_{}'.format(variable)] + traveltime[0]*source_graph['{}'.format(variable)][idx] + traveltime[1]*neighbour_graph['{}'.format(variable)][idx]])
+                return objs
+            else:
+                objs = np.array([source_graph['shortest_{}'.format(variable)] + traveltime[0]*source_graph['{}'.format(variable)], source_graph['shortest_{}'.format(variable)] + traveltime[0]*source_graph['{}'.format(variable)] + traveltime[1]*neighbour_graph['{}'.format(variable)]])
+                return objs
 
     def _neighbour_cost(self, wpt_name, minimum_objective_index):
         """
-            FILL
+            Determines the neighbour cost from a source cellbox to all of its neighbours.
+            These are then used to update the edge values in the dijkstra graph.
         """
         # Determining the nearest neighbour index for the cell
         source_graph   = self.dijkstra_info[wpt_name].loc[minimum_objective_index]
 
         # Looping over idx
         for idx in range(len(source_graph['case'])):
             indx = source_graph['neighbourIndex'][idx]
@@ -350,57 +429,56 @@
             case = source_graph['case'][idx]
 
             # Applying Newton curve to determine crossing point
             cost_func    = self.cost_func(source_graph=source_graph, neighbour_graph=neighbour_graph, case=case,
                                           unit_shipspeed='km/hr', unit_time=self.unit_time,
                                           zerocurrents=self.zero_currents)
             # Updating the Dijkstra graph with the new information
-            traveltime, crossing_points,cell_points = cost_func.value()
+            traveltime, crossing_points,cell_points,case = cost_func.value()
 
             source_graph['neighbourTravelLegs'].append(traveltime)
             source_graph['neighbourCrossingPoints'].append(np.array(crossing_points))
 
             # Using neighbourhood cost determine objective function value
-            value = self._objective_value(self.config['Route_Info']['objective_function'], source_graph,
-                                          neighbour_graph, traveltime)
-            if value[1] < neighbour_graph['shortest_{}'.format(self.config['Route_Info']['objective_function'])]:
-                for vrbl in self.config['Route_Info']['path_variables']:
-                    value = self._objective_value(vrbl, source_graph, neighbour_graph,traveltime)
+            value = self._objective_value(self.config['objective_function'], source_graph,neighbour_graph, traveltime, case)
+            if value[1] < neighbour_graph['shortest_{}'.format(self.config['objective_function'])]:
+                for vrbl in self.config['path_variables']:
+                    value = self._objective_value(vrbl, source_graph, neighbour_graph,traveltime, case)
                     neighbour_graph['shortest_{}'.format(vrbl)] = value[1]
                     neighbour_graph['path_{}'.format(vrbl)]   = source_graph['path_{}'.format(vrbl)] + list(value)
                 neighbour_graph['pathIndex']  = source_graph['pathIndex']  + [indx]
                 neighbour_graph['pathPoints'] = source_graph['pathPoints'] + [list(crossing_points)] + [list(cell_points)]
                 self.dijkstra_info[wpt_name].loc[indx] = neighbour_graph
 
         self.dijkstra_info[wpt_name].loc[minimum_objective_index] = source_graph
 
     def _dijkstra(self, wpt_name):
         """
-            FILL
+            Runs dijkstra across the whole of the domain.
         """
         # Including only the End Waypoints defined by the user
         wpts = self.mesh['waypoints'][self.mesh['waypoints']['Name'].isin(self.end_waypoints)]
         
         # Initialising zero traveltime at the source location
         source_index = int(self.mesh['waypoints'][self.mesh['waypoints']['Name'] == wpt_name]['index'])
 
-        for vrbl in self.config['Route_Info']['path_variables']:
+        for vrbl in self.config['path_variables']:
             self.dijkstra_info[wpt_name].loc[source_index, 'shortest_{}'.format(vrbl)] = 0.0
         self.dijkstra_info[wpt_name].loc[source_index, 'pathIndex'].append(source_index)
         
         # # Updating Dijkstra as long as all the waypoints are not visited or for full graph
-        if self.config['Route_Info']['early_stopping_criterion']:
+        if self.config['early_stopping_criterion']:
             stopping_criterion_indices = wpts['index']
         else:
             stopping_criterion_indices = self.dijkstra_info[wpt_name].index
 
         while (self.dijkstra_info[wpt_name].loc[stopping_criterion_indices, 'positionLocked'] == False).any():
 
             # Determining the index of the minimum objective function that has not been visited
-            minimum_objective_index = self.dijkstra_info[wpt_name][self.dijkstra_info[wpt_name]['positionLocked'] == False]['shortest_{}'.format(self.config['Route_Info']['objective_function'])].idxmin()
+            minimum_objective_index = self.dijkstra_info[wpt_name][self.dijkstra_info[wpt_name]['positionLocked'] == False]['shortest_{}'.format(self.config['objective_function'])].idxmin()
   
             # Finding the cost of the nearest neighbours from the source cell (Sc)
             self._neighbour_cost(wpt_name,minimum_objective_index)
 
             # Updating Position to be locked
             self.dijkstra_info[wpt_name].loc[minimum_objective_index, 'positionLocked'] = True
 
@@ -417,15 +495,16 @@
             raise Exception('No destination waypoints defined that are accessible')
 
         # Initialising the Dijkstra Info Dictionary
         for wpt in self.source_waypoints:
             self.dijkstra_info[wpt] = copy.copy(self.neighbour_graph)
 
         # 
-        logging.info('============= Dijkstr Path Creation ============\n')
+        logging.info('============= Dijkstra Path Creation ============')
+        logging.info(' - Objective = {} '.format(self.config['objective_function']))
 
         for wpt in self.source_waypoints:
             logging.info('--- Processing Waypoint = {} ---'.format(wpt))
             if len(self.mesh['waypoints'][self.mesh['waypoints']['Name'] == wpt]) == 0:
                 logging.warning('{} not in accessible waypoints, continuing'.format(wpt))
                 continue
             elif (len(self.mesh['waypoints']['Name'] == wpt) > 0) and (len(self.mesh['waypoints']['Name'] != wpt) == 0):
@@ -434,24 +513,43 @@
             else:
                 self._dijkstra(wpt)
 
 
         # Using Dijkstra Graph compute path and meta information to all end_waypoints
         self.paths = self._dijkstra_paths(self.source_waypoints, self.end_waypoints)
         self.mesh['paths'] = self.paths
-        for ii in range(len(self.mesh['paths']['features'])):
-            self.mesh['paths']['features'][ii]['properties']['times'] = [str(ii) for ii in (pd.to_datetime(self.mesh['config']['Mesh_info']['Region']['startTime']) + pd.to_timedelta(self.mesh['paths']['features'][ii]['properties']['traveltime'],unit='days'))]
 
     def compute_smoothed_routes(self):
         """
             Using the previously constructed Dijkstra paths smooth the paths to remove mesh features 
             `paths` will be updated in the output JSON
         """
-        maxiter     = self.config['Route_Info']['smooth_path']['max_iteration_number']
-        minimumDiff = self.config['Route_Info']['smooth_path']['minimum_difference']
+        if 'max_iteration_number' not in self.config['smooth_path']:
+            maxiter = 1e4
+        else:
+            maxiter     = self.config['smooth_path']['max_iteration_number']
+
+        if 'minimum_iterations' not in self.config['smooth_path']:
+            minimum_iterations = 50
+        else:
+            minimum_iterations = self.config['smooth_path']['minimum_iterations']
+
+
+        if 'minimum_difference' not in self.config['smooth_path']:
+            minimumDiff = 1e-4
+        else: 
+            minimumDiff = self.config['smooth_path']['minimum_difference']
+
+        # Minimum Difference = 1e-4
+        # Minimum Iterations = 50
+        # Max Iteration Number = 1e4
+
+
+
+        # 
 
         # 
         SmoothedPaths = []
         geojson = {}
         geojson['type'] = "FeatureCollection"
 
         if len(self.paths['features']) == 0:
@@ -495,90 +593,79 @@
                 # try:
 
                 # while iter < nc.pathIter:
                 pbar = tqdm(np.arange(nc.pathIter))
 
                 # Determining the computational time averaged across all pairs
                 self.allDist = []
-                self.allDist2 = []
 
                 self.nc = nc
-
+                self.all_crossing_points = []
                 for iter in pbar:
+                    self.all_crossing_points += [nc.CrossingDF]
                     nc.previousDF = copy.deepcopy(nc.CrossingDF)
                     id = 0
                     while id <= (len(nc.CrossingDF) - 3):
-                        #try:
+                        
+                        
+                        # -- Updating the crossing point
                         nc.triplet = nc.CrossingDF.iloc[id:id+3]
-                
-                        nc._updateCrossingPoint()
+                        nc._updateCrossingPoint(iter)
                         self.nc = nc
-
-                        # -- Horseshoe Case Detection -- 
-                        nc._horseshoe()
-
-                        # -- Removing reseverse cases                    
-                        nc._reverseCase()
-                        # except:
-                        #     break
-
-                        id += 1+nc.id
+                        id += 1
 
                     if  id <= (len(nc.CrossingDF) - 3):
                         print('Path Smoothing Failed!')
                         break
 
-
                     self.nc = nc
 
-                    nc._mergePoint()
+                    #nc._mergePoint()
                     self.nc = nc
                     iter+=1
+
+                    
                         
                     # Stop optimisation if the points are within some minimum difference
                     if len(nc.previousDF) == len(nc.CrossingDF):
-                        Dist = np.mean(np.sqrt((nc.previousDF['cx'].astype(float) - nc.CrossingDF['cx'].astype(float))**2 + (nc.previousDF['cy'].astype(float) - nc.CrossingDF['cy'].astype(float))**2))
+                        Dist = np.max(np.sqrt((nc.previousDF['cx'].astype(float) - nc.CrossingDF['cx'].astype(float))**2 + (nc.previousDF['cy'].astype(float) - nc.CrossingDF['cy'].astype(float))**2))
                         self.allDist.append(Dist)
                         pbar.set_description("Mean Difference = {}".format(Dist))
-
-                        if (Dist==np.min(self.allDist)) and len(np.where(abs(self.allDist - np.min(self.allDist)) < 1e-3)[0]) > 500:
-                            logging.info('{} iterations - dDist={}  - early stopping terminated oscilation, returning lowest misfit path - Type 1'.format(iter,Dist))
-                            break
-                        if (Dist < minimumDiff) and (Dist != 0.0):
+                        if (Dist < minimumDiff) and (iter>=minimum_iterations):
                             logging.info('{} iterations - dDist={}'.format(iter, Dist))
                             break
-                    # else:
-                    #     if 'Dist' in locals():
-                    #         self.allDist2.append(Dist)
-                    #         if (np.sum((np.array(self.allDist2) - Dist)[-5:]) < 1e-6) and (iter>50) and len(self.allDist2)>50:
-                    #             if self.verbose:
-                    #                 print('{} iterations - dDist={}  - early stopping terminated oscilation, returning lowest misfit path - Type 2'.format(iter,Dist))
-                    #             break
+
+                if iter == nc.pathIter:
+                    logging.info('Maximum Iteration Met - Returning Last Path'.format(iter, Dist))
+                    nc.CrossingDF = self.all_crossing_points[-1]
 
 
 
+                # ------ Smooth Path Values -----
+                # Given a smoothed route path now determine the along path parameters.
+                variables      = nc.objective_function(nc.CrossingDF)
+                TravelTimeLegs = variables['traveltime']['path_values']
+                DistanceLegs   = variables['distance']['path_values'] 
+                pathIndex      = variables['cell_index']['path_values'] 
+                FuelLegs       = variables['fuel']['path_values'] 
+                SpeedLegs      = variables['speed']['path_values'] 
 
-                # Determining the traveltime 
-                TravelTimeLegs,DistanceLegs,pathIndex = nc.objective_function()
-                FuelLegs  = TravelTimeLegs*self.neighbour_graph['fuel'].loc[pathIndex]
-                SpeedLegs = self.neighbour_graph['speed'].loc[pathIndex]
 
+                # ------ Saving Output in a standard form to be saved ------
                 SmoothedPath ={}
                 SmoothedPath['type'] = 'Feature'
                 SmoothedPath['geometry'] = {}
                 SmoothedPath['geometry']['type'] = "LineString"
                 SmoothedPath['geometry']['coordinates'] = nc.CrossingDF[['cx','cy']].to_numpy().tolist()            
                 SmoothedPath['properties'] = {}
                 SmoothedPath['properties']['from'] = Path['properties']['from']
                 SmoothedPath['properties']['to']   = Path['properties']['to']
-                SmoothedPath['properties']['traveltime'] = np.cumsum(TravelTimeLegs).tolist() 
-                SmoothedPath['properties']['fuel']  = np.cumsum(FuelLegs).tolist()
-                SmoothedPath['properties']['distance'] = np.cumsum(DistanceLegs).tolist()
-                SmoothedPath['properties']['speed'] = SpeedLegs.tolist()
+                SmoothedPath['properties']['traveltime'] = list(TravelTimeLegs)
+                SmoothedPath['properties']['fuel']       = list(FuelLegs)
+                SmoothedPath['properties']['distance']   = list(DistanceLegs)
+                SmoothedPath['properties']['speed']      = list(SpeedLegs)
                 SmoothedPaths.append(SmoothedPath)
                 geojson['features'] = SmoothedPaths
                 self.smoothed_paths = geojson
                 self.mesh['paths'] = self.smoothed_paths
-        for ii in range(len(self.mesh['paths']['features'])):
-            self.mesh['paths']['features'][ii]['properties']['times'] = [str(ii) for ii in (pd.to_datetime(self.mesh['config']['Mesh_info']['Region']['startTime']) + pd.to_timedelta(self.mesh['paths']['features'][ii]['properties']['traveltime'],unit='days'))]
```

### Comparing `polar_route-0.0.15/polar_route/vessel_performance.py` & `polar_route-0.1.0/polar_route/vessel_performance/vessels/SDA.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,286 +1,299 @@
-"""
-The VesselPerformance class deals with all the vehicle specific features of the meshed environment model. It uses the
-specific vessel parameters defined in the config to determine which cells in the mesh are inaccessible to a given
-vehicle, either based on elevation or sea ice concentration, and determines vessel performance characteristics, such as
-the speed and fuel consumption, based on the content of the cellboxes.
+from polar_route.mesh_generation.aggregated_cellBox import AggregatedCellBox
+from polar_route.vessel_performance.vessels.abstract_ship import AbstractShip
+import numpy as np
+import logging
 
-The input to the class is the mesh object produced by the CellGrid class in json format and it returns a modified mesh
-in the same format via the VesselPerformance.to_json method.
+class SDA(AbstractShip):
+    """
+        Vessel class with methods specifically designed to model the performance of the British Antarctic Survey
+        research and supply ship, the RRS Sir David Attenborough (SDA)
+    """
+    def __init__(self, params):
+        """
+            Args:
+                params (dict): vessel parameters from the vessel config file
+        """
+        super().__init__(params)
 
-Example:
-    An example of how to use this code can be executed by running the following::
+        self.force_limit = self.vessel_params['ForceLimit']
+        self.beam = self.vessel_params['Beam']
+        self.hull_type = self.vessel_params['HullType']
 
-        import json
-        from RoutePlanner.CellGrid import CellGrid
-        from RoutePlanner.vessel_performance import VesselPerformance
+    def model_speed(self, cellbox):
+        """
+            Method to determine the maximum speed that the SDA can traverse the given cell
+            Args:
+                cellbox (AggregatedCellBox): input cell from environmental mesh
 
-        with open("config.json", 'r') as f:
-            cfg = json.load(f)
+            Returns:
+                cellbox (AggregatedCellBox): updated cell with speed values
+        """
 
-        mesh = CellGrid(cfg)
-        mesh_json = mesh.to_json()
+        logging.debug(f"Calculating new speed for cellbox {cellbox.id} based on SDA resistance models")
+        speed = cellbox.agg_data['speed']
+        ice_resistance = None
+
+        if all(k in cellbox.agg_data for k in ("SIC", "thickness", "density")):
+            logging.debug("Adjusting speed according to ice resistance model")
+            if cellbox.agg_data['SIC'] == 0.0:
+                ice_resistance = 0.
+                speed = self.max_speed
+            elif cellbox.agg_data['SIC'] > self.max_ice:
+                speed = 0.0
+                ice_resistance = np.inf
+            else:
+                ice_resistance = self.ice_resistance(cellbox)
+                if ice_resistance > self.force_limit:
+                    speed = self.invert_resistance(cellbox)
+                    cellbox.agg_data['speed'] = speed
+                    ice_resistance = self.ice_resistance(cellbox)
+                else:
+                    speed = self.max_speed
+        else:
+            logging.debug("No resistance data available, no speed adjustment necessary")
 
-        vp = VesselPerformance(mesh_json)
+        logging.debug("Creating speed array")
+        cellbox.agg_data['speed'] = [speed for x in range(8)]
 
-        vehicle_mesh = vp.to_json()
-"""
-import logging
-import json
-import numpy as np
-import pandas as pd
+        if ice_resistance is not None:
+            cellbox.agg_data['ice resistance'] = ice_resistance
 
-from polar_route.utils import timed_call
+        return cellbox
 
+    def model_fuel(self, cellbox):
+        """
+            Method to determine the fuel consumption rate of the SDA in a given cell
+            Args:
+                cellbox (AggregatedCellBox): input cell from environmental mesh
 
-class VesselPerformance:
-    """
-        Class for modelling the vessel performance.
-        Takes a mesh as input in json format and modifies it to include vessel specifics.
+            Returns:
+                cellbox (AggregatedCellBox): updated cell with fuel consumption values
+        """
+        logging.debug(f"Calculating fuel requirements in cell {cellbox.id}")
 
-        Attributes:
-            mesh (dict): A dictionary containing all the mesh information
-            config (dict): The config used to generate the input mesh
-            mesh_df (DataFrame): The cellbox information from the mesh stored in a pandas DataFrame
-            vessel_params (dict): The vessel specific information contained within the config
+        cellbox = self.model_resistance(cellbox)
 
-    """
-    def __init__(self, mesh_json):
-        """
-            Constructs the VesselPerformance class from a given input mesh in json format which is then modified
-            according to the vessel parameters defined in the config.
+        cellbox.agg_data['fuel'] = [fuel_eq(cellbox.agg_data['speed'][i], r)
+                                    for i, r in enumerate(cellbox.agg_data['resistance'])]
+        return cellbox
 
-            Args:
-                mesh_json (dict): The input mesh containing the cellboxes and neighbour graph as well as the config used
-                to generate the mesh.
-        """
-        logging.info("Initialising vessel performance...")
-        self.mesh = mesh_json
-        self.config = self.mesh['config']
-        self.mesh_df = pd.DataFrame(self.mesh['cellboxes']).set_index('id')
-        self.vessel_params = self.config['Vessel']
-
-        # Check for NaNs in input and zero them if present
-        if self.mesh_df.isnull().values.any():
-            logging.debug("NaNs present in input mesh, setting all NaN values to zero")
-            self.mesh_df = self.mesh_df.fillna(0.)
-
-        # Identifying land and extreme ice cells then removing them from the neighbour graph
-        self.land()
-        self.extreme_ice()
-        self.inaccessible_nodes()
-
-        # Checking if the speed is defined in the input mesh
-        if 'speed' not in self.mesh_df:
-            logging.debug(f'No speed in mesh, assigning default value of {self.vessel_params["Speed"]} '
-                          f'{self.vessel_params["Unit"]} from config')
-            self.mesh_df['speed'] = self.vessel_params["Speed"]
-
-        # Modify speed based on ice resistance
-        self.speed()
-
-        # Calculate fuel usage based on speed and ice resistance
-        self.fuel()
-
-        # Check again for NaNs and zero them then warn if present
-        if self.mesh_df.isnull().values.any():
-            logging.warning("NaNs present in output mesh, setting all NaN values to zero!")
-            self.mesh_df = self.mesh_df.fillna(0.)
-
-        # Updating the mesh indexing and cellboxes
-        self.mesh_df['id'] = self.mesh_df.index
-        self.mesh['cellboxes'] = self.mesh_df.to_dict('records')
 
-    def to_json(self):
+    def model_resistance(self, cellbox):
         """
-            Method to return the modified mesh in json format.
+            Method to determine the resistance force acting on the SDA in a given cell
+            Args:
+                cellbox (AggregatedCellBox): input cell from environmental mesh
 
             Returns:
-                j_mesh (dict): a dictionary representation of the modified mesh.
+                cellbox (AggregatedCellBox): updated cell with resistance values
         """
-        j_mesh = json.loads(json.dumps(self.mesh))
-        return j_mesh
 
-    def land(self):
-        """
-            Method to determine which cells are land based on configured minimum depth.
-        """
-        if 'elevation' not in self.mesh_df:
-            logging.warning("No elevation data in mesh, no cells will be marked as land!")
-            self.mesh_df['land'] = False
+        # Include ice resistance if present
+        if 'ice resistance' in cellbox.agg_data:
+            ice_resistance = [cellbox.agg_data['ice resistance'] for x in range(8)]
         else:
-            self.mesh_df['land'] = self.mesh_df['elevation'] > self.vessel_params['MinDepth']
-            logging.debug(f"{self.mesh_df['land'].sum()} cells inaccessible due to land")
+            ice_resistance = [0, 0, 0, 0, 0, 0, 0, 0]
 
-    def extreme_ice(self):
-        """
-            Method to determine which cells are inaccessible based on configured max ice concentration.
-        """
-        if 'SIC' not in self.mesh_df:
-            logging.info("No sea ice concentration data in mesh")
-            self.mesh_df['ext_ice'] = False
+        # Calculate wind resistance if wind data present:
+        if 'u10' in cellbox.agg_data and 'v10' in cellbox.agg_data:
+            cellbox = calc_wind(cellbox)
+            cellbox.agg_data['resistance'] = [cellbox.agg_data['wind resistance'][i] + ice_resistance[i] for i in range(8)]
         else:
-            self.mesh_df['ext_ice'] = self.mesh_df['SIC'] > self.vessel_params['MaxIceExtent']
-            logging.debug(f"{self.mesh_df['ext_ice'].sum()} cells inaccessible due to extreme ice")
+            logging.debug("No wind data present, wind resistance will not be calculated")
+            cellbox.agg_data['resistance'] = ice_resistance
 
-    @timed_call
-    def inaccessible_nodes(self):
-        """
-            Method to determine which nodes are inaccessible and remove them from the neighbour graph.
-        """
-        logging.info("Determining which nodes are inaccessible due to land and ice")
-        inaccessible = self.mesh_df[(self.mesh_df['land']) | (self.mesh_df['ext_ice'])]
-        inaccessible_idx = list(inaccessible.index)
+        return cellbox
 
-        self.mesh['neighbour_graph'] = self.remove_nodes(self.mesh['neighbour_graph'], inaccessible_idx)
-
-    def ice_resistance(self, velocity, area, thickness, density):
+    def ice_resistance(self, cellbox):
         """
-            Method to find the ice resistance force at a given speed in a given cell.
-
-            Args:
+            Method to find the ice resistance force acting on the SDA at a given speed in a given cell.
+            The input cellbox should contain the following values:
                 velocity (float): The speed of the vessel in km/h
-                area (float): The average sea ice concentration in the cell as a percentage
+                sic (float): The average sea ice concentration in the cell as a percentage
                 thickness (float): The average ice thickness in the cell in m
                 density (float): The average ice density in the cell in kg/m^3
 
+            Args:
+                cellbox (AggregatedCellBox): input cell from environmental mesh
+
             Returns:
                 resistance (float): Resistance force in N
         """
+
+        velocity = cellbox.agg_data['speed']
+        sic = cellbox.agg_data['SIC']
+        thickness = cellbox.agg_data['thickness']
+        density = cellbox.agg_data['density']
+
+        # If there's no ice then return zero
+        if not sic:
+            return 0.
+
         # Model parameters for different hull types
         hull_params = {'slender': [4.4, -0.8267, 2.0], 'blunt': [16.1, -1.7937, 3]}
 
-        hull = self.vessel_params['HullType']
-        beam = self.vessel_params['Beam']
+        hull = self.hull_type
+        beam = self.beam
         kparam, bparam, nparam = hull_params[hull]
         gravity = 9.81  # m/s-2
 
         speed = velocity * (5. / 18.)  # assume km/h and convert to m/s
 
-        froude = speed / np.sqrt(gravity * area / 100 * thickness)
+        froude = speed / np.sqrt(gravity * (sic / 100) * thickness)
         resistance = 0.5 * kparam * (froude ** bparam) * density * beam * thickness * (speed ** 2) * (
-                    (area / 100) ** nparam)
+                    (sic / 100) ** nparam)
         return resistance
 
-    def inverse_resistance(self, area, thickness, density):
+    def invert_resistance(self, cellbox):
         """
             Method to find the vessel speed that keeps the ice resistance force below a given threshold in a given cell.
-
-            Args:
-                area (float): The average sea ice concentration in the cell as a percentage
+            The input cellbox should contain the following values:
+                sic (float): The average sea ice concentration in the cell as a percentage
                 thickness (float): The average ice thickness in the cell in m
                 density (float): The average ice density in the cell in kg/m^3
 
+            Args:
+                cellbox (AggregatedCellBox): input cell from environmental mesh
+
             Returns:
-                speed (float): Safe vessel speed in km/h
+                new_speed (float): Safe vessel speed in km/h
         """
+
+        sic = cellbox.agg_data['SIC']
+        thickness = cellbox.agg_data['thickness']
+        density = cellbox.agg_data['density']
+
+        # If there's no ice then return max speed
+        if not sic:
+            return self.max_speed
+
         # Model parameters for different hull types
         hull_params = {'slender': [4.4, -0.8267, 2.0], 'blunt': [16.1, -1.7937, 3]}
         # force_limit (float): Resistance force value that should not be exceeded in N
-        force_limit = self.vessel_params['ForceLimit']
+        force_limit = self.force_limit
 
-        hull = self.vessel_params['HullType']
-        beam = self.vessel_params['Beam']
+        hull = self.hull_type
+        beam = self.beam
         kparam, bparam, nparam = hull_params[hull]
         gravity = 9.81  # m/s-2
 
-        vexp = 2 * force_limit / (kparam * density * beam * thickness * ((area / 100) ** nparam) * (
-                    gravity * thickness * area / 100) ** -(bparam / 2))
+        vexp = 2 * force_limit / (kparam * density * beam * thickness * ((sic / 100) ** nparam) * (
+                gravity * thickness * sic / 100) ** -(bparam / 2))
 
         vms = vexp ** (1 / (2.0 + bparam))
-        speed = vms * (18. / 5.)  # convert from m/s to km/h
+        new_speed = vms * (18. / 5.)  # convert from m/s to km/h
 
-        return speed
+        return new_speed
 
-    @timed_call
-    def speed(self):
-        """
-            Method to compile the new speeds calculated based on the ice resistance into the mesh.
-        """
-        logging.info("Calculating new speeds based on resistance models")
-
-        if all(k in self.mesh_df for k in ("SIC", "thickness", "density")):
-            logging.info("Adjusting speed according to ice resistance model")
-            self.mesh_df['ice resistance'] = np.nan
-            for idx, row in self.mesh_df.iterrows():
-                if row['SIC'] == 0.0:
-                    self.mesh_df.loc[idx, 'speed'] = self.vessel_params['Speed']
-                    self.mesh_df.loc[idx, 'ice resistance'] = 0.0
-                elif row['SIC'] > self.vessel_params['MaxIceExtent']:
-                    self.mesh_df.loc[idx, 'speed'] = 0.0
-                    self.mesh_df.loc[idx, 'ice resistance'] = np.inf
-                else:
-                    rp = self.ice_resistance(self.vessel_params['Speed'], row['SIC'], row['thickness'], row['density'])
-                    if rp > self.vessel_params['ForceLimit']:
-                        new_speed = self.inverse_resistance(row['SIC'], row['thickness'], row['density'])
-                        rp = self.ice_resistance(new_speed, row['SIC'], row['thickness'], row['density'])
-                        self.mesh_df.loc[idx, 'speed'] = new_speed
-                        self.mesh_df.loc[idx, 'ice resistance'] = rp
-                    else:
-                        self.mesh_df.loc[idx, 'speed'] = self.vessel_params['Speed']
-                        self.mesh_df.loc[idx, 'ice resistance'] = rp
-        else:
-            logging.info("No resistance data available, no speed adjustment necessary")
 
-    def speed_simple(self):
-        """
-            Method to calculate the speed based on the sea ice concentration using a simple toy model.
-        """
-        self.mesh_df['speed'] = (1 - np.sqrt(self.mesh_df['SIC'] / 100)) * \
-                                        self.vessel_params['Speed']
+def fuel_eq(speed, resistance):
+    """
+        Equation to calculate the fuel consumption in tons/day given the speed in km/h and the resistance force in N
+        Args:
+            speed (float): the SDA's speed in km/h
+            resistance (float): the resistance force in N
 
-    @timed_call
-    def fuel(self):
-        """
-            Method to calculate the fuel usage in tons per day based on speed in km/h and ice resistance in N.
-        """
-        logging.info("Calculating fuel requirements in each cell")
+        Returns:
+            fuel (float): the fuel consumption in tons/day
+    """
+    # Assume no effect from "negative resistance" (e.g. when tailwind is stronger than ice resistance)
+    if resistance < 0:
+        resistance = 0.
+    fuel = (0.00137247 * speed ** 2 - 0.0029601 * speed + 0.25290433
+          + 7.75218178e-11 * resistance ** 2 + 6.48113363e-06 * resistance) * 24.0
+    return fuel
 
-        if 'ice resistance' in self.mesh_df:
-            self.mesh_df['fuel'] = (0.00137247 * self.mesh_df['speed'] ** 2 - 0.0029601 *
-                                    self.mesh_df['speed'] + 0.25290433
-                                    + 7.75218178e-11 * self.mesh_df['ice resistance'] ** 2
-                                    + 6.48113363e-06 * self.mesh_df['ice resistance']) * 24.0
-        else:
-            self.mesh_df['fuel'] = (0.00137247 * self.mesh_df['speed'] ** 2 - 0.0029601 *
-                                    self.mesh_df['speed'] + 0.25290433) * 24.0
 
-    def remove_nodes(self, neighbour_graph, inaccessible_nodes):
-        """
-            Method to remove a list of inaccessible nodes from a given neighbour graph.
+def c_wind(rel_ang):
+    """
+        Function to return the wind resistance coefficient for some relative angle between wind and travel directions.
+    """
+    cs = -1 * np.array([-0.94, -0.77, -0.42, -0.48, -0.17, 0.30, 0.34])
+    angles = np.array([0., np.pi / 6., np.pi / 3., np.pi / 2., 2 * np.pi / 3., 5 * np.pi / 6., np.pi])
+    return np.interp(rel_ang, angles, cs)
 
-            Args:
-                neighbour_graph (dict): A dictionary containing indexes of cellboxes and how they are connected
 
-                {
-                    'index':{
-                        '1':[index,...],
-                        '2':[index,...],
-                        '3':[index,...],
-                        '4':[index,...],
-                        '-1':[index,...],
-                        '-2':[index,...],
-                        '-3':[index,...],
-                        '-4':[index,...]
-                    },
-                    'index':{...},
-                    ...
-                }
+def wind_mag_dir(cellbox, va):
+    """
+        Function that returns the relative wind speed and direction given the speed and heading of the vessel
+        and the easterly and northerly components of the true wind vector. Speeds in m/s.
+    """
+    vs = cellbox.agg_data['speed'][0]*0.277778
+    uw = cellbox.agg_data['u10']
+    vw = cellbox.agg_data['v10']
 
-                inaccessible_nodes (list): A list of indexes to be removed from the neighbour_graph
+    # Define wind vector
+    w_vec = np.array([uw, vw])
+
+    # Find vessel vector in component form
+    uv, vv = vs * np.sin(va), vs * np.cos(va)
+    v_vec = np.array([uv, vv])
+
+    # Find apparent wind vector
+    aw_vec = w_vec - v_vec
+
+    # Find magnitude of apparent wind
+    ws = np.linalg.norm(aw_vec)
+
+    # Define unit vectors for dot product
+    if vs:
+        unit_v = v_vec / vs
+    else:
+        unit_v = [0., 0.]
+    if ws:
+        unit_aw = aw_vec / ws
+    else:
+        return 0., 0.
+
+    # Calculate dot product and find angle
+    dp = np.dot(unit_v, unit_aw)
+    ang = np.arccos(-1 * dp)
+
+    return ws, ang
+
+
+def wind_resistance(v_speed, w_speed, rel_ang):
+    """
+        Function to calculate the wind resistance given the wind speed and direction and the vessel speed.
+    """
+    a = 750.
+    rho = 1.225
+
+    wind_res = 0.5 * rho * (w_speed**2) * a * c_wind(rel_ang) - 0.5 * rho * (v_speed ** 2) * a * c_wind(0)
+
+    return wind_res
+
+
+def calc_wind(cellbox):
+    """
+        Function to calculate the wind resistance as well as the relative wind speed and angle for a vessel traversing a
+        cell with 8 different equally spaced angular headings.
+
+        Args:
+            cellbox (AggregatedCellBox): input cell from environmental mesh
+
+        Returns:
+            cellbox (AggregatedCellBox): updated cell with wind information
+    """
+
+    logging.debug(f"Calculating wind resistance in cellbox {cellbox.id}")
+
+    wind_res = [0, 0, 0, 0, 0, 0, 0, 0]
+    rel_wind_speed = [0, 0, 0, 0, 0, 0, 0, 0]
+    rel_wind_angle = [0, 0, 0, 0, 0, 0, 0, 0]
+
+    heads = [np.pi/4, np.pi/2, 3*np.pi/4, np.pi, 5*np.pi/4, 3*np.pi/2, 7*np.pi/4, 0.]
+    for i, head in enumerate(heads):
+        rel_wind_speed[i], rel_wind_angle[i] = wind_mag_dir(cellbox, head)
+        wind_res[i] = wind_resistance(cellbox.agg_data['speed'][i]*0.277778, rel_wind_speed[i],
+                                           rel_wind_angle[i]) # assume km/h and convert to m/s
+
+    cellbox.agg_data['wind resistance'] = wind_res
+    cellbox.agg_data['relative wind speed'] = rel_wind_speed
+    cellbox.agg_data['relative wind angle'] = rel_wind_angle
+
+    return cellbox
 
-            Returns:
-                accessibility_graph (dict): A new neighbour graph with the inaccessible nodes removed
-        """
-        logging.debug(f"Removing {len(inaccessible_nodes)} nodes from the neighbour graph")
-        accessibility_graph = neighbour_graph.copy()
 
-        for node in accessibility_graph.keys():
-            for case in accessibility_graph[node].keys():
-                for inaccessible_node in inaccessible_nodes:
-                    if int(inaccessible_node) in accessibility_graph[node][case]:
-                        accessibility_graph[node][case].remove(int(inaccessible_node))
 
-        for node in inaccessible_nodes:
-            accessibility_graph.pop(node)
 
-        return accessibility_graph
```

### Comparing `polar_route-0.0.15/polar_route.egg-info/PKG-INFO` & `polar_route-0.1.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
-Name: polar-route
-Version: 0.0.15
+Name: polar_route
+Version: 0.1.0
 Summary: PolarRoute: Long-distance maritime polar route planning taking into account complex changing environmental conditions
 Home-page: https://www.github.com/antarctica
-Author: Jonathan Smith, Samuel Hall, George Coombs, James Byrne,  Michael Thorne, Maria Fox
+Author: Jonathan Smith, Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry, James Byrne, Michael Thorne, Maria Fox
 Author-email: jonsmi@bas.ac.uk
-Maintainer: Jonathan Smith, Samuel Hall, George Coombs, James Byrne,  Michael Thorne, Maria Fox
+Maintainer: Jonathan Smith, Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry, James Byrne, Michael Thorne, Maria Fox
 Maintainer-email: jonsmi@bas.ac.uk
 License: MIT
-Platform: UNKNOWN
 Classifier: 
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Topic :: Scientific/Engineering
 Classifier: 
 Description-Content-Type: text/markdown
 Provides-Extra: tests
+License-File: LICENSE
 
 ![](logo.jpg)
 
 <a href="https://colab.research.google.com/drive/12D-CN10X7xAcXn_df0zNLHtdiiXxZVkz?usp=sharing"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab" alt="Colab">
 <a href="https://antarctica.github.io/PolarRoute/"><img src="https://img.shields.io/badge/Manual%20-github.io%2FPolarRoute%2F-red" alt="Manual Page">
 <a href="https://pypi.org/project/polar-route/"><img src="https://img.shields.io/pypi/v/polar-route" alt="PyPi">
 <a href="https://github.com/antarctica/PolarRoute/tags"><img src="https://img.shields.io/github/v/tag/antarctica/PolarRoute" alt="Release Tag"></a>
@@ -46,20 +46,40 @@
 
  Pip: 
 ```
 pip install polar-route
 ```
 
 ## Required Data sources
-Polar-route has been built to work with a variety of open-source climactic data sources. 
-A list of supported data sources and there associated data-loaders is given in the 
+Polar-route has been built to work with a variety of open-source atmospheric and oceanographic data sources. 
+A list of supported data sources and their associated data-loaders is given in the 
 'Data Loaders' section of the manual
 
+## Documentation
+Sphinx is used to generate documentation for this project. The dependencies can be installed through pip:
+```
+pip install sphinx sphinx_markdown_builder sphinx_rtd_theme rinohtype
+```
+When updating the docs, run the following command within the PolarRoute directory to recompile.
+```
+sphinx-build -b html ./docs/source ./docs/html
+```
+Sometimes the cache needs to be cleared for internal links to update. If facing this problem, run this from the PolarRoute directory.
+```
+rm -r docs/build/.doctrees/
+```
 ## Developers
-Jonathan Smith, Samuel Hall, George Coombs, James Byrne,  Michael Thorne, Maria Fox
+Jonathan Smith, Samuel Hall, George Coombs, James Byrne,  Michael Thorne, Maria Fox, Harrison Abbot, Ayat Fekry
+
+## Collaboration
+We are currently assessing the best pratice for collaboration on the codebase, until then please contact [marfox@bas.ac.uk](marfox@bas.ac.uk) or [jonsmi@bas.ac.uk](jonsmi@bas.ac.uk) for further info.
+
 
 ## License
-This software is licensed under a MIT license. For more information please see the attached ``LICENSE`` file.
+This software is licensed under a MIT license, but request users cite our publication.  
+
+Jonathan D. Smith, Samuel Hall, George Coombs, James Byrne, Michael A. S. Thorne,  J. Alexander Brearley, Derek Long, Michael Meredith, Maria Fox,  (2022), Autonomous Passage Planning for a Polar Vessel, arXiv, https://arxiv.org/abs/2209.02389
+
+For more information please see the attached ``LICENSE`` file. 
 
 [version]: https://img.shields.io/PolarRoute/v/datadog-metrics.svg?style=flat-square
 [downloads]: https://img.shields.io/PolarRoute/dm/datadog-metrics.svg?style=flat-square
-
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
-Metadata-Version: 2.1 Name: polar-route Version: 0.0.15 Summary: PolarRoute:
+Metadata-Version: 2.1 Name: polar_route Version: 0.1.0 Summary: PolarRoute:
 Long-distance maritime polar route planning taking into account complex
 changing environmental conditions Home-page: https://www.github.com/antarctica
-Author: Jonathan Smith, Samuel Hall, George Coombs, James Byrne, Michael
-Thorne, Maria Fox Author-email: jonsmi@bas.ac.uk Maintainer: Jonathan Smith,
-Samuel Hall, George Coombs, James Byrne, Michael Thorne, Maria Fox Maintainer-
-email: jonsmi@bas.ac.uk License: MIT Platform: UNKNOWN Classifier: Classifier:
-Development Status :: 3 - Alpha Classifier: Intended Audience :: Science/
-Research Classifier: Intended Audience :: System Administrators Classifier:
-License :: OSI Approved :: MIT License Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.7 Classifier: Topic :: Scientific/
-Engineering Classifier: Description-Content-Type: text/markdown Provides-Extra:
-tests ![](logo.jpg) [Open_In_Colab]_[Manual_Page]_[PyPi]_[Release_Tag]_[Issues]
+Author: Jonathan Smith, Samuel Hall, George Coombs, Harrison Abbot, Ayat Fekry,
+James Byrne, Michael Thorne, Maria Fox Author-email: jonsmi@bas.ac.uk
+Maintainer: Jonathan Smith, Samuel Hall, George Coombs, Harrison Abbot, Ayat
+Fekry, James Byrne, Michael Thorne, Maria Fox Maintainer-email:
+jonsmi@bas.ac.uk License: MIT Classifier: Classifier: Development Status :: 3 -
+Alpha Classifier: Intended Audience :: Science/Research Classifier: Intended
+Audience :: System Administrators Classifier: License :: OSI Approved :: MIT
+License Classifier: Natural Language :: English Classifier: Operating System ::
+OS Independent Classifier: Programming Language :: Python Classifier:
+Programming Language :: Python :: 3 Classifier: Programming Language :: Python
+:: 3.7 Classifier: Topic :: Scientific/Engineering Classifier: Description-
+Content-Type: text/markdown Provides-Extra: tests License-File: LICENSE ![]
+(logo.jpg) [Open_In_Colab]_[Manual_Page]_[PyPi]_[Release_Tag]_[Issues]_
 [License]_#_PolarRoute_>_PolarRoute_is_a_long-distance_maritime_polar_route
 planning,_taking_into_account_complex_changing_environmental_conditions._The
 codebase_allows_the_construction_of_optimised_routes_through_three_main_stages:
 discrete_modelling_of_the_environmental_conditions_using_a_non-uniform_mesh,
 the_construction_of_mesh-optimal_paths,_and_physics_informed_path_smoothing._In
 order_to_account_for_different_vehicle_properties_we_construct_a_series_of_data
 driven_functions_that_can_be_applied_to_the_environmental_mesh_to_determine_the
@@ -24,14 +25,28 @@
 representing_these_quantities_graphically_and_geospatially._##_Installation_The
 PolarRoute_software_requires_GDAL_files_to_be_installed._The_PolarRoute
 software_can_be_installed_on_Windows_by_running_the_required_wheels_for_GDAL
 and_FIONA._MOre_information_can_be_found_in_the_manual_pages_linked_above._Once
 these_requirements_are_met_then_the_software_can_be_installed_by:_Github:_```
 python_setup.py_install_```_Pip:_```_pip_install_polar-route_```_##_Required
 Data_sources_Polar-route_has_been_built_to_work_with_a_variety_of_open-source
-climactic_data_sources._A_list_of_supported_data_sources_and_there_associated
-data-loaders_is_given_in_the_'Data_Loaders'_section_of_the_manual_##_Developers
+atmospheric_and_oceanographic_data_sources._A_list_of_supported_data_sources
+and_their_associated_data-loaders_is_given_in_the_'Data_Loaders'_section_of_the
+manual_##_Documentation_Sphinx_is_used_to_generate_documentation_for_this
+project._The_dependencies_can_be_installed_through_pip:_```_pip_install_sphinx
+sphinx_markdown_builder_sphinx_rtd_theme_rinohtype_```_When_updating_the_docs,
+run_the_following_command_within_the_PolarRoute_directory_to_recompile._```
+sphinx-build_-b_html_./docs/source_./docs/html_```_Sometimes_the_cache_needs_to
+be_cleared_for_internal_links_to_update._If_facing_this_problem,_run_this_from
+the_PolarRoute_directory._```_rm_-r_docs/build/.doctrees/_```_##_Developers
 Jonathan_Smith,_Samuel_Hall,_George_Coombs,_James_Byrne,_Michael_Thorne,_Maria
-Fox_##_License_This_software_is_licensed_under_a_MIT_license._For_more
-information_please_see_the_attached_``LICENSE``_file._[version]:_https://
-img.shields.io/PolarRoute/v/datadog-metrics.svg?style=flat-square_[downloads]:
-https://img.shields.io/PolarRoute/dm/datadog-metrics.svg?style=flat-square_
+Fox,_Harrison_Abbot,_Ayat_Fekry_##_Collaboration_We_are_currently_assessing_the
+best_pratice_for_collaboration_on_the_codebase,_until_then_please_contact_
+[marfox@bas.ac.uk](marfox@bas.ac.uk)_or_[jonsmi@bas.ac.uk](jonsmi@bas.ac.uk)
+for_further_info._##_License_This_software_is_licensed_under_a_MIT_license,_but
+request_users_cite_our_publication._Jonathan_D._Smith,_Samuel_Hall,_George
+Coombs,_James_Byrne,_Michael_A._S._Thorne,_J._Alexander_Brearley,_Derek_Long,
+Michael_Meredith,_Maria_Fox,_(2022),_Autonomous_Passage_Planning_for_a_Polar
+Vessel,_arXiv,_https://arxiv.org/abs/2209.02389_For_more_information_please_see
+the_attached_``LICENSE``_file._[version]:_https://img.shields.io/PolarRoute/v/
+datadog-metrics.svg?style=flat-square_[downloads]:_https://img.shields.io/
+PolarRoute/dm/datadog-metrics.svg?style=flat-square_
```

### Comparing `polar_route-0.0.15/setup.py` & `polar_route-0.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from setuptools import setup, find_packages
 
 import polar_route
-
+import polar_route.dataloaders
+import polar_route.mesh_generation
+import polar_route.vessel_performance
 
 def get_content(filename):
     with open(filename, "r") as fh:
         return fh.read()
 
 
 requirements = get_content("requirements.txt")
@@ -36,15 +38,16 @@
         Programming Language :: Python :: 3.7
         Topic :: Scientific/Engineering
     """.split('\n')],
     entry_points={
         'console_scripts': [
             "create_mesh=polar_route.cli:create_mesh_cli",
             "add_vehicle=polar_route.cli:add_vehicle_cli",
-            "optimise_routes=polar_route.cli:optimise_routes_cli"],
+            "optimise_routes=polar_route.cli:optimise_routes_cli",
+            "export_mesh=polar_route.cli:export_mesh_cli"],
     },
     keywords=[],
     packages=find_packages(),
     install_requires=requirements,
     tests_require=["pytest"],
     extras_require={
         "tests": get_content("tests/requirements.txt"),
```


# Comparing `tmp/PyTrack-lib-2.0.6.tar.gz` & `tmp/PyTrack-lib-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTrack-lib-2.0.6.tar", last modified: Thu Oct 20 21:51:33 2022, max compression
+gzip compressed data, was "PyTrack-lib-2.0.7.tar", last modified: Tue Apr 18 22:49:05 2023, max compression
```

## Comparing `PyTrack-lib-2.0.6.tar` & `PyTrack-lib-2.0.7.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:51:33.897440 PyTrack-lib-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1686 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4410 2022-10-20 21:51:33.897440 PyTrack-lib-2.0.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:51:33.893440 PyTrack-lib-2.0.6/PyTrack_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4410 2022-10-20 21:51:33.000000 PyTrack-lib-2.0.6/PyTrack_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-10-20 21:51:33.000000 PyTrack-lib-2.0.6/PyTrack_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-20 21:51:33.000000 PyTrack-lib-2.0.6/PyTrack_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-10-20 21:51:33.000000 PyTrack-lib-2.0.6/PyTrack_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-10-20 21:51:33.000000 PyTrack-lib-2.0.6/PyTrack_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3633 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:51:33.893440 PyTrack-lib-2.0.6/pytrack/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:51:33.893440 PyTrack-lib-2.0.6/pytrack/analytics/
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/analytics/plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     4535 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/analytics/video.py
--rw-r--r--   0 runner    (1001) docker     (121)    15220 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/analytics/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:51:33.897440 PyTrack-lib-2.0.6/pytrack/graph/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6434 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/graph/distance.py
--rw-r--r--   0 runner    (1001) docker     (121)     3014 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/graph/download.py
--rw-r--r--   0 runner    (1001) docker     (121)    11598 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     3186 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/graph/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:51:33.897440 PyTrack-lib-2.0.6/pytrack/matching/
--rw-r--r--   0 runner    (1001) docker     (121)      213 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/matching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4937 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/matching/candidate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/matching/cleaning.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/matching/matcher.py
--rw-r--r--   0 runner    (1001) docker     (121)     2891 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/matching/mpmatching.py
--rw-r--r--   0 runner    (1001) docker     (121)     6035 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/matching/mpmatching_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-20 21:51:33.897440 PyTrack-lib-2.0.6/pytrack/video/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/video/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/video/create_video.py
--rw-r--r--   0 runner    (1001) docker     (121)     3382 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/pytrack/video/streetview.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-20 21:51:33.897440 PyTrack-lib-2.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-10-20 21:51:22.000000 PyTrack-lib-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:49:05.904626 PyTrack-lib-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-04-18 22:48:51.000000 PyTrack-lib-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-18 22:49:05.904626 PyTrack-lib-2.0.7/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:49:05.900626 PyTrack-lib-2.0.7/PyTrack_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-18 22:49:05.000000 PyTrack-lib-2.0.7/PyTrack_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-18 22:49:05.000000 PyTrack-lib-2.0.7/PyTrack_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 22:49:05.000000 PyTrack-lib-2.0.7/PyTrack_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-04-18 22:49:05.000000 PyTrack-lib-2.0.7/PyTrack_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 22:49:05.000000 PyTrack-lib-2.0.7/PyTrack_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-04-18 22:48:51.000000 PyTrack-lib-2.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:49:05.900626 PyTrack-lib-2.0.7/pytrack/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:49:05.900626 PyTrack-lib-2.0.7/pytrack/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/analytics/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/analytics/video.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/analytics/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:49:05.904626 PyTrack-lib-2.0.7/pytrack/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/graph/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/graph/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11598 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/graph/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:49:05.904626 PyTrack-lib-2.0.7/pytrack/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/matching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/matching/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/matching/cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/matching/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/matching/mpmatching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/matching/mpmatching_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 22:49:05.904626 PyTrack-lib-2.0.7/pytrack/video/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/video/create_video.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/pytrack/video/streetview.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 22:49:05.904626 PyTrack-lib-2.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-04-18 22:48:52.000000 PyTrack-lib-2.0.7/setup.py
```

### Comparing `PyTrack-lib-2.0.6/LICENSE` & `PyTrack-lib-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTrack-lib-2.0.6/PKG-INFO` & `PyTrack-lib-2.0.7/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: PyTrack-lib
-Version: 2.0.6
-Summary: a Map-Matching-based Python Toolbox for Vehicle Trajectory Reconstruction
-Home-page: https://github.com/cosbidev/PyTrack
-Author: Matteo Tortora
-Author-email: m.tortora@unicampus.it
-License: BSD-3-Clause-Clear
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: GIS
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align="center">
 <img src="https://raw.githubusercontent.com/cosbidev/PyTrack/main/logo/pytracklogo.svg" width="300">
 </h1><br>
 
 -----------------
 
 # PyTrack: a Map-Matching-based Python Toolbox for Vehicle Trajectory Reconstruction
@@ -32,14 +13,30 @@
 [![PyPI downloads](https://img.shields.io/pypi/dm/pytrack-lib?label=PyPI%20downloads)](https://pypi.org/project/PyTrack-lib/)
 [![Anaconda downloads](https://img.shields.io/conda/dn/conda-forge/pytrack?label=conda%20downloads)](https://anaconda.org/conda-forge/pytrack)
 
 ## What is it?
 **PyTrack** is a Python package that integrate the recorded GPS coordinates with data provided by the open-source OpenStreetMap (OSM). 
 PyTrack can serve the intelligent transport research, e.g. to reconstruct the video of a vehicle’s route by exploiting available data and without equipping it with camera sensors, to update the urban road network, and so on.
 
+If you use PyTrack in your work, please cite the journal article.
+
+**Citation info**: M. Tortora, E. Cordelli and P. Soda, "[PyTrack: a Map-Matching-based Python Toolbox for Vehicle Trajectory Reconstruction](https://ieeexplore.ieee.org/document/9927417)," in IEEE Access, vol. 10, pp. 112713-112720, 2022, doi: 10.1109/ACCESS.2022.3216565.
+
+```latex
+@ARTICLE{mtpytrack,  
+      author={Tortora, Matteo and Cordelli, Ermanno and Soda, Paolo},
+      journal={IEEE Access}, 
+      title={PyTrack: A Map-Matching-Based Python Toolbox for Vehicle Trajectory Reconstruction}, 
+      year={2022},
+      volume={10},
+      number={},
+      pages={112713-112720},
+      doi={10.1109/ACCESS.2022.3216565}}
+```
+
 ## Main Features
 The following are the main features that PyTrack includes:
 - Generation of the street network graph using geospatial data from OpenStreetMap
 - Map-matching
 - Data cleaning
 - Video reconstruction of the GPS route
 - Visualisation and analysis capabilities
```

#### html2text {}

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1 Name: PyTrack-lib Version: 2.0.6 Summary: a Map-Matching-
-based Python Toolbox for Vehicle Trajectory Reconstruction Home-page: https://
-github.com/cosbidev/PyTrack Author: Matteo Tortora Author-email:
-m.tortora@unicampus.it License: BSD-3-Clause-Clear Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent Classifier: Topic :: Scientific/
-Engineering :: GIS Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Scientific/Engineering :: Physics Classifier: Topic ::
-Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
-Engineering :: Information Analysis Description-Content-Type: text/markdown
-License-File: LICENSE
      ****** [https://raw.githubusercontent.com/cosbidev/PyTrack/main/logo/
                             pytracklogo.svg] ******
 
 ----------------- # PyTrack: a Map-Matching-based Python Toolbox for Vehicle
 Trajectory Reconstruction [![All platforms](https://dev.azure.com/conda-forge/
 feedstock-builds/_apis/build/status/pytrack-feedstock?branchName=main)](https:/
 /dev.azure.com/conda-forge/feedstock-builds/_build/
@@ -26,28 +15,37 @@
 pypi.org/project/PyTrack-lib/) [![Anaconda downloads](https://img.shields.io/
 conda/dn/conda-forge/pytrack?label=conda%20downloads)](https://anaconda.org/
 conda-forge/pytrack) ## What is it? **PyTrack** is a Python package that
 integrate the recorded GPS coordinates with data provided by the open-source
 OpenStreetMap (OSM). PyTrack can serve the intelligent transport research, e.g.
 to reconstruct the video of a vehicleâs route by exploiting available data
 and without equipping it with camera sensors, to update the urban road network,
-and so on. ## Main Features The following are the main features that PyTrack
-includes: - Generation of the street network graph using geospatial data from
-OpenStreetMap - Map-matching - Data cleaning - Video reconstruction of the GPS
-route - Visualisation and analysis capabilities ## Getting Started ###
-Installation The source code is currently hosted on GitHub at: https://
-github.com/cosbidev/PyTrack. PyTrack can be installed using*: ```sh # conda
-conda install pytrack ``` ```sh # or PyPI pip install PyTrack-lib ``` **for Mac
-m1 users, it is recommended to use conda in order to be able to install all
-dependencies.* ## Documentation Checkout the official [documentation](https://
-pytrack-lib.readthedocs.io/en/latest). Besides, [here](https://github.com/
-cosbidev/PyTrack/tree/main/examples) you can see some examples of the
-application of the library. ## Examples ### Map-Matching To see the map-
-matching feature of PyTrack in action please go to [map-matching documentation]
-(https://pytrack-lib.readthedocs.io/en/latest/notebooks/map-matching.html).
+and so on. If you use PyTrack in your work, please cite the journal article.
+**Citation info**: M. Tortora, E. Cordelli and P. Soda, "[PyTrack: a Map-
+Matching-based Python Toolbox for Vehicle Trajectory Reconstruction](https://
+ieeexplore.ieee.org/document/9927417)," in IEEE Access, vol. 10, pp. 112713-
+112720, 2022, doi: 10.1109/ACCESS.2022.3216565. ```latex @ARTICLE{mtpytrack,
+author={Tortora, Matteo and Cordelli, Ermanno and Soda, Paolo}, journal={IEEE
+Access}, title={PyTrack: A Map-Matching-Based Python Toolbox for Vehicle
+Trajectory Reconstruction}, year={2022}, volume={10}, number={}, pages={112713-
+112720}, doi={10.1109/ACCESS.2022.3216565}} ``` ## Main Features The following
+are the main features that PyTrack includes: - Generation of the street network
+graph using geospatial data from OpenStreetMap - Map-matching - Data cleaning -
+Video reconstruction of the GPS route - Visualisation and analysis capabilities
+## Getting Started ### Installation The source code is currently hosted on
+GitHub at: https://github.com/cosbidev/PyTrack. PyTrack can be installed
+using*: ```sh # conda conda install pytrack ``` ```sh # or PyPI pip install
+PyTrack-lib ``` **for Mac m1 users, it is recommended to use conda in order to
+be able to install all dependencies.* ## Documentation Checkout the official
+[documentation](https://pytrack-lib.readthedocs.io/en/latest). Besides, [here]
+(https://github.com/cosbidev/PyTrack/tree/main/examples) you can see some
+examples of the application of the library. ## Examples ### Map-Matching To see
+the map-matching feature of PyTrack in action please go to [map-matching
+documentation](https://pytrack-lib.readthedocs.io/en/latest/notebooks/map-
+matching.html).
                                 [map-matching]
 ### Video reconstruction of the itinerary
                         [video_track] [video_seg_track]
 ## Contributing to PyTrack All contributions, bug reports, bug fixes,
 documentation improvements, enhancements, and ideas are welcome. ## Author
 Created by [Matteo Tortora](https://mtortora-ai.github.io) - feel free to
 contact me!  ## License PyTrack is distributed under a [BSD-3-Clause-Clear
```

### Comparing `PyTrack-lib-2.0.6/PyTrack_lib.egg-info/PKG-INFO` & `PyTrack-lib-2.0.7/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTrack-lib
-Version: 2.0.6
+Version: 2.0.7
 Summary: a Map-Matching-based Python Toolbox for Vehicle Trajectory Reconstruction
 Home-page: https://github.com/cosbidev/PyTrack
 Author: Matteo Tortora
 Author-email: m.tortora@unicampus.it
 License: BSD-3-Clause-Clear
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -32,14 +32,30 @@
 [![PyPI downloads](https://img.shields.io/pypi/dm/pytrack-lib?label=PyPI%20downloads)](https://pypi.org/project/PyTrack-lib/)
 [![Anaconda downloads](https://img.shields.io/conda/dn/conda-forge/pytrack?label=conda%20downloads)](https://anaconda.org/conda-forge/pytrack)
 
 ## What is it?
 **PyTrack** is a Python package that integrate the recorded GPS coordinates with data provided by the open-source OpenStreetMap (OSM). 
 PyTrack can serve the intelligent transport research, e.g. to reconstruct the video of a vehicle’s route by exploiting available data and without equipping it with camera sensors, to update the urban road network, and so on.
 
+If you use PyTrack in your work, please cite the journal article.
+
+**Citation info**: M. Tortora, E. Cordelli and P. Soda, "[PyTrack: a Map-Matching-based Python Toolbox for Vehicle Trajectory Reconstruction](https://ieeexplore.ieee.org/document/9927417)," in IEEE Access, vol. 10, pp. 112713-112720, 2022, doi: 10.1109/ACCESS.2022.3216565.
+
+```latex
+@ARTICLE{mtpytrack,  
+      author={Tortora, Matteo and Cordelli, Ermanno and Soda, Paolo},
+      journal={IEEE Access}, 
+      title={PyTrack: A Map-Matching-Based Python Toolbox for Vehicle Trajectory Reconstruction}, 
+      year={2022},
+      volume={10},
+      number={},
+      pages={112713-112720},
+      doi={10.1109/ACCESS.2022.3216565}}
+```
+
 ## Main Features
 The following are the main features that PyTrack includes:
 - Generation of the street network graph using geospatial data from OpenStreetMap
 - Map-matching
 - Data cleaning
 - Video reconstruction of the GPS route
 - Visualisation and analysis capabilities
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: PyTrack-lib Version: 2.0.6 Summary: a Map-Matching-
+Metadata-Version: 2.1 Name: PyTrack-lib Version: 2.0.7 Summary: a Map-Matching-
 based Python Toolbox for Vehicle Trajectory Reconstruction Home-page: https://
 github.com/cosbidev/PyTrack Author: Matteo Tortora Author-email:
 m.tortora@unicampus.it License: BSD-3-Clause-Clear Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent Classifier: Topic :: Scientific/
 Engineering :: GIS Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Physics Classifier: Topic ::
@@ -26,28 +26,37 @@
 pypi.org/project/PyTrack-lib/) [![Anaconda downloads](https://img.shields.io/
 conda/dn/conda-forge/pytrack?label=conda%20downloads)](https://anaconda.org/
 conda-forge/pytrack) ## What is it? **PyTrack** is a Python package that
 integrate the recorded GPS coordinates with data provided by the open-source
 OpenStreetMap (OSM). PyTrack can serve the intelligent transport research, e.g.
 to reconstruct the video of a vehicleâs route by exploiting available data
 and without equipping it with camera sensors, to update the urban road network,
-and so on. ## Main Features The following are the main features that PyTrack
-includes: - Generation of the street network graph using geospatial data from
-OpenStreetMap - Map-matching - Data cleaning - Video reconstruction of the GPS
-route - Visualisation and analysis capabilities ## Getting Started ###
-Installation The source code is currently hosted on GitHub at: https://
-github.com/cosbidev/PyTrack. PyTrack can be installed using*: ```sh # conda
-conda install pytrack ``` ```sh # or PyPI pip install PyTrack-lib ``` **for Mac
-m1 users, it is recommended to use conda in order to be able to install all
-dependencies.* ## Documentation Checkout the official [documentation](https://
-pytrack-lib.readthedocs.io/en/latest). Besides, [here](https://github.com/
-cosbidev/PyTrack/tree/main/examples) you can see some examples of the
-application of the library. ## Examples ### Map-Matching To see the map-
-matching feature of PyTrack in action please go to [map-matching documentation]
-(https://pytrack-lib.readthedocs.io/en/latest/notebooks/map-matching.html).
+and so on. If you use PyTrack in your work, please cite the journal article.
+**Citation info**: M. Tortora, E. Cordelli and P. Soda, "[PyTrack: a Map-
+Matching-based Python Toolbox for Vehicle Trajectory Reconstruction](https://
+ieeexplore.ieee.org/document/9927417)," in IEEE Access, vol. 10, pp. 112713-
+112720, 2022, doi: 10.1109/ACCESS.2022.3216565. ```latex @ARTICLE{mtpytrack,
+author={Tortora, Matteo and Cordelli, Ermanno and Soda, Paolo}, journal={IEEE
+Access}, title={PyTrack: A Map-Matching-Based Python Toolbox for Vehicle
+Trajectory Reconstruction}, year={2022}, volume={10}, number={}, pages={112713-
+112720}, doi={10.1109/ACCESS.2022.3216565}} ``` ## Main Features The following
+are the main features that PyTrack includes: - Generation of the street network
+graph using geospatial data from OpenStreetMap - Map-matching - Data cleaning -
+Video reconstruction of the GPS route - Visualisation and analysis capabilities
+## Getting Started ### Installation The source code is currently hosted on
+GitHub at: https://github.com/cosbidev/PyTrack. PyTrack can be installed
+using*: ```sh # conda conda install pytrack ``` ```sh # or PyPI pip install
+PyTrack-lib ``` **for Mac m1 users, it is recommended to use conda in order to
+be able to install all dependencies.* ## Documentation Checkout the official
+[documentation](https://pytrack-lib.readthedocs.io/en/latest). Besides, [here]
+(https://github.com/cosbidev/PyTrack/tree/main/examples) you can see some
+examples of the application of the library. ## Examples ### Map-Matching To see
+the map-matching feature of PyTrack in action please go to [map-matching
+documentation](https://pytrack-lib.readthedocs.io/en/latest/notebooks/map-
+matching.html).
                                 [map-matching]
 ### Video reconstruction of the itinerary
                         [video_track] [video_seg_track]
 ## Contributing to PyTrack All contributions, bug reports, bug fixes,
 documentation improvements, enhancements, and ideas are welcome. ## Author
 Created by [Matteo Tortora](https://mtortora-ai.github.io) - feel free to
 contact me!  ## License PyTrack is distributed under a [BSD-3-Clause-Clear
```

### Comparing `PyTrack-lib-2.0.6/PyTrack_lib.egg-info/SOURCES.txt` & `PyTrack-lib-2.0.7/PyTrack_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyTrack-lib-2.0.6/pytrack/analytics/video.py` & `PyTrack-lib-2.0.7/pytrack/analytics/video.py`

 * *Files identical despite different names*

### Comparing `PyTrack-lib-2.0.6/pytrack/analytics/visualization.py` & `PyTrack-lib-2.0.7/pytrack/analytics/visualization.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import random
 from inspect import signature
 
 import folium
 import matplotlib.pyplot as plt
 import networkx as nx
 from shapely.geometry import LineString
 
@@ -116,14 +117,36 @@
                 self._children.pop(key)
         children = self._children
         self.__init__(self.location, tiles=self.tiles)
         self.options = self.options
         for k, v in children.items():
             self.add_child(v)
 
+    def _layer_control_exist(self):
+        # Check if a layer control already exists on the map
+        self.layer_control_exist = False
+        for child in self._children:
+            if child.startswith('layer_control'):
+                self.layer_control_exist = True
+                break
+
+    def _manage_layer_control(self):
+        # Check if a layer control already exists on the map
+        self._layer_control_exist()
+
+        # Add a new layer control if one doesn't exist
+        if self.layer_control_exist:
+            del self._children[next(k for k in self._children.keys() if k.startswith('layer_control'))]
+            self.add_child(folium.LayerControl())
+            self._render_reset()
+
+        # Add a new layer control if one doesn't exist
+        else:
+            folium.LayerControl().add_to(self)
+
     def add_graph(self, G, plot_nodes=False, edge_color="#3388ff", edge_width=3,
                   edge_opacity=1, radius=1.7, node_color="red", fill=True, fill_color=None,
                   fill_opacity=1):
         """ Add the road network graph created with ``pytrack.graph.graph.graph_from_bbox`` method
 
         Parameters
         ----------
@@ -171,15 +194,16 @@
         if plot_nodes:
             fg_point = folium.FeatureGroup(name='Graph vertices', show=True)
             self.add_child(fg_point)
             for point, osmid in zip(nodes.geometry, nodes.osmid):
                 folium.Circle(location=(point.y, point.x), popup=f"osmid: {osmid}", radius=radius, **node_attr).add_to(
                     fg_point)
 
-        folium.LayerControl().add_to(self)
+        # Update layer_control if it exists, otherwise create it
+        self._manage_layer_control()
 
     def draw_candidates(self, candidates, radius, point_radius=1, point_color="black", point_fill=True,
                         point_fill_opacity=1, area_weight=1, area_color="black", area_fill=True, area_fill_opacity=0.2,
                         cand_radius=1, cand_color="orange", cand_fill=True, cand_fill_opacity=1):
         """ Draw the candidate nodes of the HMM matcher
 
         Parameters
@@ -235,17 +259,16 @@
                 if cand_type:
                     folium.Circle(location=cand, popup=popup, radius=2, color="yellow", fill=True,
                                   fill_opacity=1).add_to(fg_cands)
                 else:
                     folium.Circle(location=cand, popup=popup, radius=cand_radius, color=cand_color, fill=cand_fill,
                                   fill_opacity=cand_fill_opacity).add_to(fg_cands)
 
-        del self._children[next(k for k in self._children.keys() if k.startswith('layer_control'))]
-        self.add_child(folium.LayerControl())
-        self._render_reset()
+        # Update layer_control if it exists, otherwise create it
+        self._manage_layer_control()
 
     def draw_path(self, G, trellis, predecessor, path_name="Matched path", path_color="green", path_weight=4,
                   path_opacity=1):
         """ Draw the map-matched path
 
         Parameters
         ----------
@@ -274,17 +297,57 @@
         edge_attr["color"] = path_color
         edge_attr["weight"] = path_weight
         edge_attr["opacity"] = path_opacity
 
         edge = [(lat, lng) for lng, lat in LineString([G.nodes[node]["geometry"] for node in path_elab]).coords]
         folium.PolyLine(locations=edge, **edge_attr).add_to(fg_matched)
 
-        del self._children[next(k for k in self._children.keys() if k.startswith('layer_control'))]
-        self.add_child(folium.LayerControl())
-        self._render_reset()
+        # Update layer_control if it exists, otherwise create it
+        self._manage_layer_control()
+
+    def add_geojson(self, geojson_data_list, styles=None, layer_names=None):
+        """ Add a GeoJSON layer to a Folium map object.
+
+        Parameters
+        ----------
+        geojson_data_list : list of str, dict, or file
+            The list of GeoJSON data as strings, dictionaries, or files.
+        styles : list of function, optional
+            The list of style functions for each GeoJSON layer. Each function should take a 'feature' argument
+            and return a dictionary of style options. If None, a random color will be assigned to each layer.
+            Default is None.
+        layer_names : list of str, optional
+            The list of names for each GeoJSON layer. If None, each layer will be named "Layer i" where i is
+            its index in geojson_data_list. If provided, the length of layer_names must match the length of
+            geojson_data_list. Default is None.
+        """
+        # Generate a random color for each layer if no style is provided
+        if styles is None:
+            styles = [lambda feature, color=f"#{random.randint(0, 0xFFFFFF):06x}": {
+                "color": color,
+                "weight": 2,
+                "opacity": 0.8,
+                "fillColor": color,
+                "fillOpacity": 0.5
+            } for _ in geojson_data_list]
+
+        # Create a FeatureGroup to aggregate the GeoJSON layers
+        feature_group = folium.FeatureGroup(name="GeoJSON Layers")
+        self.add_child(feature_group)
+
+        # Create a GeoJSON layer for each input data and add to the map
+        for i, (geojson_data, style) in enumerate(zip(geojson_data_list, styles)):
+            folium.GeoJson(
+                geojson_data,
+                style_function=style,
+                name=layer_names[i] if layer_names is not None and i < len(layer_names) else f"Layer {i + 1}"
+            ).add_to(feature_group)
+
+        # Update layer_control if it exists, otherwise create it
+        self._manage_layer_control()
 
 
 def draw_trellis(T, figsize=(15, 12), dpi=300, node_size=500, font_size=8, **kwargs):
     """ Draw a trellis graph
 
     Parameters
     ----------
```

### Comparing `PyTrack-lib-2.0.6/pytrack/graph/distance.py` & `PyTrack-lib-2.0.7/pytrack/graph/distance.py`

 * *Files identical despite different names*

### Comparing `PyTrack-lib-2.0.6/pytrack/graph/download.py` & `PyTrack-lib-2.0.7/pytrack/graph/download.py`

 * *Files identical despite different names*

### Comparing `PyTrack-lib-2.0.6/pytrack/graph/graph.py` & `PyTrack-lib-2.0.7/pytrack/graph/graph.py`

 * *Files identical despite different names*

### Comparing `PyTrack-lib-2.0.6/pytrack/graph/utils.py` & `PyTrack-lib-2.0.7/pytrack/graph/utils.py`

 * *Files identical despite different names*

### Comparing `PyTrack-lib-2.0.6/pytrack/matching/candidate.py` & `PyTrack-lib-2.0.7/pytrack/matching/candidate.py`

 * *Files identical despite different names*

### Comparing `PyTrack-lib-2.0.6/pytrack/matching/cleaning.py` & `PyTrack-lib-2.0.7/pytrack/matching/cleaning.py`

 * *Files identical despite different names*

### Comparing `PyTrack-lib-2.0.6/pytrack/matching/mpmatching.py` & `PyTrack-lib-2.0.7/pytrack/matching/mpmatching.py`

 * *Files identical despite different names*

### Comparing `PyTrack-lib-2.0.6/pytrack/matching/mpmatching_utils.py` & `PyTrack-lib-2.0.7/pytrack/matching/mpmatching_utils.py`

 * *Files identical despite different names*

### Comparing `PyTrack-lib-2.0.6/pytrack/video/create_video.py` & `PyTrack-lib-2.0.7/pytrack/video/create_video.py`

 * *Files identical despite different names*

### Comparing `PyTrack-lib-2.0.6/pytrack/video/streetview.py` & `PyTrack-lib-2.0.7/pytrack/video/streetview.py`

 * *Files identical despite different names*

### Comparing `PyTrack-lib-2.0.6/setup.py` & `PyTrack-lib-2.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='PyTrack-lib',
-    version='2.0.6',
+    version='2.0.7',
     packages=setuptools.find_packages(),
     # namespace_packages=['pytrack'],
     url='https://github.com/cosbidev/PyTrack',
     license='BSD-3-Clause-Clear',
     author='Matteo Tortora',
     author_email='m.tortora@unicampus.it',
     description='a Map-Matching-based Python Toolbox for Vehicle Trajectory Reconstruction',
```


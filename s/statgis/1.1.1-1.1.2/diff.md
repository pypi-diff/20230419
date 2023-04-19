# Comparing `tmp/statgis-1.1.1.tar.gz` & `tmp/statgis-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "statgis-1.1.1.tar", max compression
+gzip compressed data, was "statgis-1.1.2.tar", max compression
```

## Comparing `statgis-1.1.1.tar` & `statgis-1.1.2.tar`

### file list

```diff
@@ -1,34 +1,20 @@
--rw-r--r--   0        0        0     1133 2023-04-15 01:57:54.839842 statgis-1.1.1/LICENSE
--rw-r--r--   0        0        0      953 2023-04-18 20:26:57.929677 statgis-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1469 2023-04-15 01:57:54.871115 statgis-1.1.1/README.md
--rw-r--r--   0        0        0      159 2023-04-15 01:57:55.092860 statgis-1.1.1/src/statgis/__init__.py
--rw-r--r--   0        0        0      283 2023-04-15 01:57:55.095862 statgis-1.1.1/src/statgis/gee/__init__.py
--rw-r--r--   0        0        0      662 2023-04-15 19:25:50.282753 statgis-1.1.1/src/statgis/gee/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4292 2023-04-18 18:36:45.403720 statgis-1.1.1/src/statgis/gee/__pycache__/classification.cpython-311.pyc
--rw-r--r--   0        0        0     8193 2023-04-18 19:53:34.000024 statgis-1.1.1/src/statgis/gee/__pycache__/landsat_functions.cpython-311.pyc
--rw-r--r--   0        0        0     4269 2023-04-18 18:37:02.000763 statgis-1.1.1/src/statgis/gee/__pycache__/river_analysis.cpython-311.pyc
--rw-r--r--   0        0        0     5220 2023-04-18 20:08:06.219058 statgis-1.1.1/src/statgis/gee/__pycache__/sample.cpython-311.pyc
--rw-r--r--   0        0        0     3303 2023-04-18 19:53:39.000491 statgis-1.1.1/src/statgis/gee/__pycache__/sentinel_functions.cpython-311.pyc
--rw-r--r--   0        0        0     2467 2023-04-18 18:37:10.082006 statgis-1.1.1/src/statgis/gee/__pycache__/shoreline_analysis.cpython-311.pyc
--rw-r--r--   0        0        0     2141 2023-04-18 18:37:12.925211 statgis-1.1.1/src/statgis/gee/__pycache__/terrain_analysis.cpython-311.pyc
--rw-r--r--   0        0        0    13396 2023-04-18 19:53:43.675907 statgis-1.1.1/src/statgis/gee/__pycache__/time_series_analysis.cpython-311.pyc
--rw-r--r--   0        0        0     5461 2023-04-18 19:54:00.302889 statgis-1.1.1/src/statgis/gee/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0        0        0     7900 2023-04-18 19:53:47.145468 statgis-1.1.1/src/statgis/gee/__pycache__/zonal_statistics.cpython-311.pyc
--rw-r--r--   0        0        0     2720 2023-04-17 22:52:39.257683 statgis-1.1.1/src/statgis/gee/classification.py
--rw-r--r--   0        0        0     6056 2023-04-18 19:37:44.895652 statgis-1.1.1/src/statgis/gee/landsat_functions.py
--rw-r--r--   0        0        0     2815 2023-04-17 23:24:07.530781 statgis-1.1.1/src/statgis/gee/river_analysis.py
--rw-r--r--   0        0        0     3943 2023-04-18 20:03:49.199286 statgis-1.1.1/src/statgis/gee/sample.py
--rw-r--r--   0        0        0     2532 2023-04-18 19:41:30.512138 statgis-1.1.1/src/statgis/gee/sentinel_functions.py
--rw-r--r--   0        0        0     1334 2023-04-17 23:25:00.413231 statgis-1.1.1/src/statgis/gee/shoreline_analysis.py
--rw-r--r--   0        0        0     1237 2023-04-17 23:31:38.297087 statgis-1.1.1/src/statgis/gee/terrain_analysis.py
--rw-r--r--   0        0        0     8975 2023-04-18 19:44:54.106465 statgis-1.1.1/src/statgis/gee/time_series_analysis.py
--rw-r--r--   0        0        0     4101 2023-04-18 19:50:59.397654 statgis-1.1.1/src/statgis/gee/utils.py
--rw-r--r--   0        0        0     5579 2023-04-18 19:52:58.304434 statgis-1.1.1/src/statgis/gee/zonal_statistics.py
--rw-r--r--   0        0        0        0 2023-04-15 01:57:55.417245 statgis-1.1.1/src/statgis/statgis.py
--rw-r--r--   0        0        0       42 2023-04-15 01:57:55.471047 statgis-1.1.1/src/statgis/statutils/__init__.py
--rw-r--r--   0        0        0      266 2023-04-15 19:26:21.949342 statgis-1.1.1/src/statgis/statutils/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4421 2023-04-15 19:26:41.745766 statgis-1.1.1/src/statgis/statutils/__pycache__/plots.cpython-311.pyc
--rw-r--r--   0        0        0     2761 2023-04-15 19:26:22.074352 statgis-1.1.1/src/statgis/statutils/__pycache__/stats.cpython-311.pyc
--rw-r--r--   0        0        0     3408 2023-04-15 04:08:25.691314 statgis-1.1.1/src/statgis/statutils/plots.py
--rw-r--r--   0        0        0     1970 2023-04-15 01:57:55.526062 statgis-1.1.1/src/statgis/statutils/stats.py
--rw-r--r--   0        0        0     2236 1970-01-01 00:00:00.000000 statgis-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1133 2023-04-15 01:57:54.839842 statgis-1.1.2/LICENSE
+-rw-r--r--   0        0        0      953 2023-04-18 23:56:11.099053 statgis-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1469 2023-04-18 23:58:40.881670 statgis-1.1.2/README.md
+-rw-r--r--   0        0        0      159 2023-04-15 01:57:55.092860 statgis-1.1.2/src/statgis/__init__.py
+-rw-r--r--   0        0        0      283 2023-04-15 01:57:55.095862 statgis-1.1.2/src/statgis/gee/__init__.py
+-rw-r--r--   0        0        0     2720 2023-04-17 22:52:39.257683 statgis-1.1.2/src/statgis/gee/classification.py
+-rw-r--r--   0        0        0     6056 2023-04-18 19:37:44.895652 statgis-1.1.2/src/statgis/gee/landsat_functions.py
+-rw-r--r--   0        0        0     2815 2023-04-17 23:24:07.530781 statgis-1.1.2/src/statgis/gee/river_analysis.py
+-rw-r--r--   0        0        0     3943 2023-04-18 20:03:49.199286 statgis-1.1.2/src/statgis/gee/sample.py
+-rw-r--r--   0        0        0     2532 2023-04-18 19:41:30.512138 statgis-1.1.2/src/statgis/gee/sentinel_functions.py
+-rw-r--r--   0        0        0     1334 2023-04-17 23:25:00.413231 statgis-1.1.2/src/statgis/gee/shoreline_analysis.py
+-rw-r--r--   0        0        0     1237 2023-04-17 23:31:38.297087 statgis-1.1.2/src/statgis/gee/terrain_analysis.py
+-rw-r--r--   0        0        0     8975 2023-04-18 19:44:54.106465 statgis-1.1.2/src/statgis/gee/time_series_analysis.py
+-rw-r--r--   0        0        0     4101 2023-04-18 19:50:59.397654 statgis-1.1.2/src/statgis/gee/utils.py
+-rw-r--r--   0        0        0     5579 2023-04-18 19:52:58.304434 statgis-1.1.2/src/statgis/gee/zonal_statistics.py
+-rw-r--r--   0        0        0        0 2023-04-15 01:57:55.417245 statgis-1.1.2/src/statgis/statgis.py
+-rw-r--r--   0        0        0       42 2023-04-15 01:57:55.471047 statgis-1.1.2/src/statgis/statutils/__init__.py
+-rw-r--r--   0        0        0     3408 2023-04-15 04:08:25.691314 statgis-1.1.2/src/statgis/statutils/plots.py
+-rw-r--r--   0        0        0     1970 2023-04-15 01:57:55.526062 statgis-1.1.2/src/statgis/statutils/stats.py
+-rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 statgis-1.1.2/PKG-INFO
```

### Comparing `statgis-1.1.1/LICENSE` & `statgis-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `statgis-1.1.1/pyproject.toml` & `statgis-1.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "statgis"
-version = "1.1.1"
+version = "1.1.2"
 description = "Tools for improve work with geospatial data in Python"
 authors = ["Sebástian Narváez-Salcedo <sanarvaezstatgis@gmail.com>", "Brayan Navarro-Londoño <brnavarrostatgis@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "<3.12,>=3.8"
 earthengine-api = ">=0.1.335"
 pandas = ">=1.3.5"
 scipy = ">=1.7.3"
 matplotlib = ">=3.2.2"
-pydata-sphinx-theme = "0.13.3"
-accessible-pygments = "0.0.4"
 
 [tool.poetry.dev-dependencies]
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.2.1"
 ipython = ">=8.8.0"
 pytest-cov = ">=4.0.0"
 jupyterlab = ">=3.5.2"
 ipykernel = ">=6.20.2"
 myst-nb = {version = "^0.17.1", python = "^3.11"}
 sphinx-autoapi = "^2.0.1"
 sphinx-rtd-theme = "^1.1.1"
 sphinxcontrib-napoleon = "^0.7"
 sphinx-material = "^0.0.35"
+pydata-sphinx-theme = "0.13.3"
+accessible-pygments = "0.0.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `statgis-1.1.1/README.md` & `statgis-1.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # StatGIS Python Package
 
 ![PyPI](https://img.shields.io/pypi/v/statgis) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/statgis?color=yellow) [![Documentation Status](https://readthedocs.org/projects/statgis/badge/?version=latest)](https://statgis.readthedocs.io/en/latest/?badge=latest)
 
-StatGIS help to the users to process and analyse satellite images in Google Earth Engine.
+StatGIS help to the users to process and analyze satellite images in Google Earth Engine.
 
 ## Installation
 
 ```bash
 $ pip install statgis
 ```
```

### Comparing `statgis-1.1.1/src/statgis/gee/classification.py` & `statgis-1.1.2/src/statgis/gee/classification.py`

 * *Files identical despite different names*

### Comparing `statgis-1.1.1/src/statgis/gee/landsat_functions.py` & `statgis-1.1.2/src/statgis/gee/landsat_functions.py`

 * *Files identical despite different names*

### Comparing `statgis-1.1.1/src/statgis/gee/river_analysis.py` & `statgis-1.1.2/src/statgis/gee/river_analysis.py`

 * *Files identical despite different names*

### Comparing `statgis-1.1.1/src/statgis/gee/sample.py` & `statgis-1.1.2/src/statgis/gee/sample.py`

 * *Files identical despite different names*

### Comparing `statgis-1.1.1/src/statgis/gee/sentinel_functions.py` & `statgis-1.1.2/src/statgis/gee/sentinel_functions.py`

 * *Files identical despite different names*

### Comparing `statgis-1.1.1/src/statgis/gee/shoreline_analysis.py` & `statgis-1.1.2/src/statgis/gee/shoreline_analysis.py`

 * *Files identical despite different names*

### Comparing `statgis-1.1.1/src/statgis/gee/terrain_analysis.py` & `statgis-1.1.2/src/statgis/gee/terrain_analysis.py`

 * *Files identical despite different names*

### Comparing `statgis-1.1.1/src/statgis/gee/time_series_analysis.py` & `statgis-1.1.2/src/statgis/gee/time_series_analysis.py`

 * *Files identical despite different names*

### Comparing `statgis-1.1.1/src/statgis/gee/utils.py` & `statgis-1.1.2/src/statgis/gee/utils.py`

 * *Files identical despite different names*

### Comparing `statgis-1.1.1/src/statgis/gee/zonal_statistics.py` & `statgis-1.1.2/src/statgis/gee/zonal_statistics.py`

 * *Files identical despite different names*

### Comparing `statgis-1.1.1/src/statgis/statutils/plots.py` & `statgis-1.1.2/src/statgis/statutils/plots.py`

 * *Files identical despite different names*

### Comparing `statgis-1.1.1/src/statgis/statutils/stats.py` & `statgis-1.1.2/src/statgis/statutils/stats.py`

 * *Files identical despite different names*

### Comparing `statgis-1.1.1/PKG-INFO` & `statgis-1.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: statgis
-Version: 1.1.1
+Version: 1.1.2
 Summary: Tools for improve work with geospatial data in Python
 License: MIT
 Author: Sebástian Narváez-Salcedo
 Author-email: sanarvaezstatgis@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: accessible-pygments (==0.0.4)
 Requires-Dist: earthengine-api (>=0.1.335)
 Requires-Dist: matplotlib (>=3.2.2)
 Requires-Dist: pandas (>=1.3.5)
-Requires-Dist: pydata-sphinx-theme (==0.13.3)
 Requires-Dist: scipy (>=1.7.3)
 Description-Content-Type: text/markdown
 
 # StatGIS Python Package
 
 ![PyPI](https://img.shields.io/pypi/v/statgis) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/statgis?color=yellow) [![Documentation Status](https://readthedocs.org/projects/statgis/badge/?version=latest)](https://statgis.readthedocs.io/en/latest/?badge=latest)
 
-StatGIS help to the users to process and analyse satellite images in Google Earth Engine.
+StatGIS help to the users to process and analyze satellite images in Google Earth Engine.
 
 ## Installation
 
 ```bash
 $ pip install statgis
 ```
```


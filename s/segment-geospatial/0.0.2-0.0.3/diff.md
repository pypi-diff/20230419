# Comparing `tmp/segment-geospatial-0.0.2.tar.gz` & `tmp/segment-geospatial-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.0.2.tar", last modified: Wed Apr 19 03:31:29 2023, max compression
+gzip compressed data, was "segment-geospatial-0.0.3.tar", last modified: Wed Apr 19 03:45:58 2023, max compression
```

## Comparing `segment-geospatial-0.0.2.tar` & `segment-geospatial-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:31:29.913509 segment-geospatial-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 03:31:18.000000 segment-geospatial-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-19 03:31:18.000000 segment-geospatial-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-19 03:31:29.913509 segment-geospatial-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-04-19 03:31:18.000000 segment-geospatial-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 03:31:18.000000 segment-geospatial-0.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:31:29.913509 segment-geospatial-0.0.2/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-19 03:31:18.000000 segment-geospatial-0.0.2/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 03:31:18.000000 segment-geospatial-0.0.2/samgeo/samgeo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:31:29.913509 segment-geospatial-0.0.2/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-04-19 03:31:29.000000 segment-geospatial-0.0.2/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 03:31:29.000000 segment-geospatial-0.0.2/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 03:31:29.000000 segment-geospatial-0.0.2/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 03:31:29.000000 segment-geospatial-0.0.2/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 03:31:29.000000 segment-geospatial-0.0.2/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-19 03:31:29.913509 segment-geospatial-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-19 03:31:18.000000 segment-geospatial-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:45:58.350235 segment-geospatial-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-19 03:45:58.350235 segment-geospatial-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:45:58.350235 segment-geospatial-0.0.3/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/samgeo/samgeo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 03:45:58.350235 segment-geospatial-0.0.3/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-04-19 03:45:58.000000 segment-geospatial-0.0.3/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-19 03:45:58.000000 segment-geospatial-0.0.3/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 03:45:58.000000 segment-geospatial-0.0.3/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 03:45:58.000000 segment-geospatial-0.0.3/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-19 03:45:58.000000 segment-geospatial-0.0.3/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-19 03:45:58.000000 segment-geospatial-0.0.3/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-19 03:45:58.350235 segment-geospatial-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-04-19 03:45:49.000000 segment-geospatial-0.0.3/setup.py
```

### Comparing `segment-geospatial-0.0.2/LICENSE` & `segment-geospatial-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.0.2/PKG-INFO` & `segment-geospatial-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.0.2
+Version: 0.0.3
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
 
 
 **Meta AI' Segment Anything Model (SAM) for Geospatial Data**
 
 
 -   Free software: MIT license
--   Documentation: https://giswqs.github.io/segment-geospatial
+-   Documentation: https://samgeo.gishub.org
     
 
 ## Features
 
 -   TODO
 
 ## Credits
```

### Comparing `segment-geospatial-0.0.2/README.md` & `segment-geospatial-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
 
 
 **Meta AI' Segment Anything Model (SAM) for Geospatial Data**
 
 
 -   Free software: MIT license
--   Documentation: https://giswqs.github.io/segment-geospatial
+-   Documentation: https://samgeo.gishub.org
     
 
 ## Features
 
 -   TODO
 
 ## Credits
```

### Comparing `segment-geospatial-0.0.2/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.0.3/segment_geospatial.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.0.2
+Version: 0.0.3
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -26,15 +26,15 @@
 [![image](https://img.shields.io/conda/vn/conda-forge/segment-geospatial.svg)](https://anaconda.org/conda-forge/segment-geospatial)
 
 
 **Meta AI' Segment Anything Model (SAM) for Geospatial Data**
 
 
 -   Free software: MIT license
--   Documentation: https://giswqs.github.io/segment-geospatial
+-   Documentation: https://samgeo.gishub.org
     
 
 ## Features
 
 -   TODO
 
 ## Credits
```

### Comparing `segment-geospatial-0.0.2/setup.py` & `segment-geospatial-0.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='samgeo',
     name='segment-geospatial',
     packages=find_packages(include=['samgeo', 'samgeo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/opengeos/segment-geospatial',
-    version='0.0.2',
+    version='0.0.3',
     zip_safe=False,
 )
```


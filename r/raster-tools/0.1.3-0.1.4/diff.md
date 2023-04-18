# Comparing `tmp/raster-tools-0.1.3.tar.gz` & `tmp/raster-tools-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster-tools-0.1.3.tar", last modified: Fri Apr 14 00:14:01 2023, max compression
+gzip compressed data, was "raster-tools-0.1.4.tar", last modified: Tue Apr 18 22:06:30 2023, max compression
```

## Comparing `raster-tools-0.1.3.tar` & `raster-tools-0.1.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-14 00:14:01.282053 raster-tools-0.1.3/
--rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster-tools-0.1.3/LICENSE
--rw-r--r--   0 fred      (1000) fred      (1000)      316 2022-08-26 20:44:14.000000 raster-tools-0.1.3/MANIFEST.in
--rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-14 00:14:01.282053 raster-tools-0.1.3/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1198 2023-04-11 21:45:35.000000 raster-tools-0.1.3/README.md
--rw-r--r--   0 fred      (1000) fred      (1000)      273 2022-08-26 20:44:14.000000 raster-tools-0.1.3/pyproject.toml
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-14 00:14:01.282053 raster-tools-0.1.3/raster_tools/
--rw-rw-r--   0 fred      (1000) fred      (1000)      934 2023-01-25 21:30:15.000000 raster-tools-0.1.3/raster_tools/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)      383 2023-01-28 03:26:22.000000 raster-tools-0.1.3/raster_tools/_compat.py
--rw-rw-r--   0 fred      (1000) fred      (1000)       22 2023-04-14 00:12:51.000000 raster-tools-0.1.3/raster_tools/_version.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7664 2023-01-04 22:54:45.000000 raster-tools-0.1.3/raster_tools/batch.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6536 2023-02-01 01:11:45.000000 raster-tools-0.1.3/raster_tools/clipping.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9647 2023-03-29 17:25:11.000000 raster-tools-0.1.3/raster_tools/creation.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1286 2022-11-29 01:39:49.000000 raster-tools-0.1.3/raster_tools/dask_utils.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-14 00:14:01.282053 raster-tools-0.1.3/raster_tools/distance/
--rw-r--r--   0 fred      (1000) fred      (1000)      427 2022-08-26 20:44:16.000000 raster-tools-0.1.3/raster_tools/distance/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6777 2022-10-21 23:01:50.000000 raster-tools-0.1.3/raster_tools/distance/_heap.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    26495 2023-01-04 22:54:45.000000 raster-tools-0.1.3/raster_tools/distance/cost_distance.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    34940 2023-04-13 22:25:41.000000 raster-tools-0.1.3/raster_tools/distance/proximity.py
--rw-r--r--   0 fred      (1000) fred      (1000)     3240 2022-12-09 03:28:15.000000 raster-tools-0.1.3/raster_tools/dtypes.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20687 2023-03-03 21:13:40.000000 raster-tools-0.1.3/raster_tools/focal.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    35261 2023-04-11 22:00:22.000000 raster-tools-0.1.3/raster_tools/general.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7149 2023-01-04 22:54:45.000000 raster-tools-0.1.3/raster_tools/io.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    12275 2023-02-15 02:21:21.000000 raster-tools-0.1.3/raster_tools/line_stats.py
--rw-r--r--   0 fred      (1000) fred      (1000)     2123 2022-10-22 00:44:28.000000 raster-tools-0.1.3/raster_tools/masking.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    46873 2023-04-11 21:59:29.000000 raster-tools-0.1.3/raster_tools/raster.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4076 2022-10-21 23:01:50.000000 raster-tools-0.1.3/raster_tools/stat_common.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    17964 2023-03-31 23:07:40.000000 raster-tools-0.1.3/raster_tools/surface.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     3163 2023-02-15 02:21:21.000000 raster-tools-0.1.3/raster_tools/utils.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    26731 2023-04-14 00:13:27.000000 raster-tools-0.1.3/raster_tools/vector.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20196 2023-04-06 21:19:23.000000 raster-tools-0.1.3/raster_tools/zonal.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-14 00:14:01.282053 raster-tools-0.1.3/raster_tools.egg-info/
--rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-14 00:14:01.000000 raster-tools-0.1.3/raster_tools.egg-info/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)     1774 2023-04-14 00:14:01.000000 raster-tools-0.1.3/raster_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)        1 2023-04-14 00:14:01.000000 raster-tools-0.1.3/raster_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-04-14 00:14:01.000000 raster-tools-0.1.3/raster_tools.egg-info/requires.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       13 2023-04-14 00:14:01.000000 raster-tools-0.1.3/raster_tools.egg-info/top_level.txt
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-14 00:14:01.282053 raster-tools-0.1.3/requirements/
--rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-01-25 21:30:15.000000 raster-tools-0.1.3/requirements/default.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       38 2023-04-14 00:14:01.282053 raster-tools-0.1.3/setup.cfg
--rw-rw-r--   0 fred      (1000) fred      (1000)     1526 2023-01-31 00:50:40.000000 raster-tools-0.1.3/setup.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-14 00:14:01.282053 raster-tools-0.1.3/tests/
--rw-rw-r--   0 fred      (1000) fred      (1000)     4072 2023-01-04 22:54:46.000000 raster-tools-0.1.3/tests/test_clipping.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     7404 2023-01-04 22:54:46.000000 raster-tools-0.1.3/tests/test_distance.py
--rw-r--r--   0 fred      (1000) fred      (1000)     1297 2022-08-26 20:44:16.000000 raster-tools-0.1.3/tests/test_distance__heap.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     8212 2023-04-14 00:09:55.000000 raster-tools-0.1.3/tests/test_distance_proximity.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    20233 2023-03-03 21:13:40.000000 raster-tools-0.1.3/tests/test_focal.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    22392 2023-02-01 19:59:47.000000 raster-tools-0.1.3/tests/test_general.py
--rw-r--r--   0 fred      (1000) fred      (1000)     7288 2023-01-28 03:48:27.000000 raster-tools-0.1.3/tests/test_line_stats.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    55226 2023-02-16 01:34:06.000000 raster-tools-0.1.3/tests/test_raster.py
--rw-r--r--   0 fred      (1000) fred      (1000)     4124 2022-08-26 20:44:16.000000 raster-tools-0.1.3/tests/test_stat_common.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     5157 2023-02-15 02:21:21.000000 raster-tools-0.1.3/tests/test_surface.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    10830 2023-01-25 02:09:19.000000 raster-tools-0.1.3/tests/test_vector.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6903 2023-04-06 20:45:48.000000 raster-tools-0.1.3/tests/test_zonal.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-18 22:06:30.142218 raster-tools-0.1.4/
+-rw-------   0 fred      (1000) fred      (1000)    35149 2022-08-26 20:44:14.000000 raster-tools-0.1.4/LICENSE
+-rw-r--r--   0 fred      (1000) fred      (1000)      316 2022-08-26 20:44:14.000000 raster-tools-0.1.4/MANIFEST.in
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-18 22:06:30.142218 raster-tools-0.1.4/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1198 2023-04-11 21:45:35.000000 raster-tools-0.1.4/README.md
+-rw-r--r--   0 fred      (1000) fred      (1000)      273 2022-08-26 20:44:14.000000 raster-tools-0.1.4/pyproject.toml
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-18 22:06:30.138218 raster-tools-0.1.4/raster_tools/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      934 2023-01-25 21:30:15.000000 raster-tools-0.1.4/raster_tools/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)      383 2023-01-28 03:26:22.000000 raster-tools-0.1.4/raster_tools/_compat.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)       22 2023-04-18 22:06:23.000000 raster-tools-0.1.4/raster_tools/_version.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7664 2023-01-04 22:54:45.000000 raster-tools-0.1.4/raster_tools/batch.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6536 2023-02-01 01:11:45.000000 raster-tools-0.1.4/raster_tools/clipping.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     9647 2023-03-29 17:25:11.000000 raster-tools-0.1.4/raster_tools/creation.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1286 2022-11-29 01:39:49.000000 raster-tools-0.1.4/raster_tools/dask_utils.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-18 22:06:30.138218 raster-tools-0.1.4/raster_tools/distance/
+-rw-r--r--   0 fred      (1000) fred      (1000)      427 2022-08-26 20:44:16.000000 raster-tools-0.1.4/raster_tools/distance/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6777 2022-10-21 23:01:50.000000 raster-tools-0.1.4/raster_tools/distance/_heap.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    26495 2023-01-04 22:54:45.000000 raster-tools-0.1.4/raster_tools/distance/cost_distance.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    34940 2023-04-13 22:25:41.000000 raster-tools-0.1.4/raster_tools/distance/proximity.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     3240 2022-12-09 03:28:15.000000 raster-tools-0.1.4/raster_tools/dtypes.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20687 2023-03-03 21:13:40.000000 raster-tools-0.1.4/raster_tools/focal.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    35261 2023-04-11 22:00:22.000000 raster-tools-0.1.4/raster_tools/general.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7149 2023-01-04 22:54:45.000000 raster-tools-0.1.4/raster_tools/io.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    12275 2023-02-15 02:21:21.000000 raster-tools-0.1.4/raster_tools/line_stats.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     2123 2022-10-22 00:44:28.000000 raster-tools-0.1.4/raster_tools/masking.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    46873 2023-04-11 21:59:29.000000 raster-tools-0.1.4/raster_tools/raster.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4076 2022-10-21 23:01:50.000000 raster-tools-0.1.4/raster_tools/stat_common.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    17964 2023-03-31 23:07:40.000000 raster-tools-0.1.4/raster_tools/surface.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     3170 2023-04-18 19:26:49.000000 raster-tools-0.1.4/raster_tools/utils.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    30306 2023-04-18 19:37:34.000000 raster-tools-0.1.4/raster_tools/vector.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20196 2023-04-06 21:19:23.000000 raster-tools-0.1.4/raster_tools/zonal.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-18 22:06:30.142218 raster-tools-0.1.4/raster_tools.egg-info/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1800 2023-04-18 22:06:30.000000 raster-tools-0.1.4/raster_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1774 2023-04-18 22:06:30.000000 raster-tools-0.1.4/raster_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)        1 2023-04-18 22:06:30.000000 raster-tools-0.1.4/raster_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-04-18 22:06:30.000000 raster-tools-0.1.4/raster_tools.egg-info/requires.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       13 2023-04-18 22:06:30.000000 raster-tools-0.1.4/raster_tools.egg-info/top_level.txt
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-18 22:06:30.142218 raster-tools-0.1.4/requirements/
+-rw-rw-r--   0 fred      (1000) fred      (1000)      139 2023-01-25 21:30:15.000000 raster-tools-0.1.4/requirements/default.txt
+-rw-rw-r--   0 fred      (1000) fred      (1000)       38 2023-04-18 22:06:30.142218 raster-tools-0.1.4/setup.cfg
+-rw-rw-r--   0 fred      (1000) fred      (1000)     1526 2023-01-31 00:50:40.000000 raster-tools-0.1.4/setup.py
+drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2023-04-18 22:06:30.142218 raster-tools-0.1.4/tests/
+-rw-rw-r--   0 fred      (1000) fred      (1000)     4072 2023-01-04 22:54:46.000000 raster-tools-0.1.4/tests/test_clipping.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     7404 2023-01-04 22:54:46.000000 raster-tools-0.1.4/tests/test_distance.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     1297 2022-08-26 20:44:16.000000 raster-tools-0.1.4/tests/test_distance__heap.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     8212 2023-04-14 00:09:55.000000 raster-tools-0.1.4/tests/test_distance_proximity.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    20233 2023-03-03 21:13:40.000000 raster-tools-0.1.4/tests/test_focal.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    22392 2023-02-01 19:59:47.000000 raster-tools-0.1.4/tests/test_general.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7288 2023-01-28 03:48:27.000000 raster-tools-0.1.4/tests/test_line_stats.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    56488 2023-04-18 19:37:34.000000 raster-tools-0.1.4/tests/test_raster.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     4124 2022-08-26 20:44:16.000000 raster-tools-0.1.4/tests/test_stat_common.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     5157 2023-02-15 02:21:21.000000 raster-tools-0.1.4/tests/test_surface.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)    10830 2023-01-25 02:09:19.000000 raster-tools-0.1.4/tests/test_vector.py
+-rw-rw-r--   0 fred      (1000) fred      (1000)     6903 2023-04-06 20:45:48.000000 raster-tools-0.1.4/tests/test_zonal.py
```

### Comparing `raster-tools-0.1.3/LICENSE` & `raster-tools-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/PKG-INFO` & `raster-tools-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `raster-tools-0.1.3/README.md` & `raster-tools-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/__init__.py` & `raster-tools-0.1.4/raster_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/batch.py` & `raster-tools-0.1.4/raster_tools/batch.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/clipping.py` & `raster-tools-0.1.4/raster_tools/clipping.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/creation.py` & `raster-tools-0.1.4/raster_tools/creation.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/dask_utils.py` & `raster-tools-0.1.4/raster_tools/dask_utils.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/distance/_heap.py` & `raster-tools-0.1.4/raster_tools/distance/_heap.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/distance/cost_distance.py` & `raster-tools-0.1.4/raster_tools/distance/cost_distance.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/distance/proximity.py` & `raster-tools-0.1.4/raster_tools/distance/proximity.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/dtypes.py` & `raster-tools-0.1.4/raster_tools/dtypes.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/focal.py` & `raster-tools-0.1.4/raster_tools/focal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/general.py` & `raster-tools-0.1.4/raster_tools/general.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/io.py` & `raster-tools-0.1.4/raster_tools/io.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/line_stats.py` & `raster-tools-0.1.4/raster_tools/line_stats.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/masking.py` & `raster-tools-0.1.4/raster_tools/masking.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/raster.py` & `raster-tools-0.1.4/raster_tools/raster.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/stat_common.py` & `raster-tools-0.1.4/raster_tools/stat_common.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/surface.py` & `raster-tools-0.1.4/raster_tools/surface.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools/utils.py` & `raster-tools-0.1.4/raster_tools/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     return xr.Dataset({"raster": raster_dataarray, "mask": mask_dataarray})
 
 
 def merge_masks(masks):
     mask = None
     for m in masks:
         if mask is None:
-            mask = m
+            mask = m.copy()
         else:
             mask |= m
     return mask
 
 
 def single_band_mappable(
     func_=None, *, no_input_chunk=False, pass_block_info=False
```

### Comparing `raster-tools-0.1.3/raster_tools/vector.py` & `raster-tools-0.1.4/raster_tools/vector.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import dask.array as da
 import dask.dataframe as dd
 import dask_geopandas as dgpd
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import rasterio as rio
+import shapely
 import xarray as xr
 from dask.delayed import delayed
 from packaging import version
 from rasterio.enums import MergeAlg
 from rasterio.env import GDALVersion
 from rasterio.features import rasterize as rio_rasterize
 
@@ -227,14 +228,33 @@
         return result
     elif _is_series(src) or _is_frame(src):
         return Vector(src)
     else:
         raise TypeError("Invalid vector input")
 
 
+def get_vector_frame(src):
+    if isinstance(src, Vector):
+        return src.data
+    elif is_str(src):
+        result = open_vectors(src)
+        if not isinstance(result, Vector):
+            # More than one layer was found
+            raise ValueError("Input source must only have 1 layer")
+        return result.data
+    elif _is_series(src) or _is_frame(src):
+        if _is_series(src):
+            src = src.to_frame("geometry")
+        if dask.is_dask_collection(src):
+            return src
+        return dgpd.from_geopandas(src, npartitions=1)
+    else:
+        raise TypeError("Invalid vector input")
+
+
 def _get_len_from_divisions(divs):
     # This should never overcount but may undercount by 1 because
     # dask.dataframe special cases the last division when creating a dataframe.
     #
     # NOTE: Dask dataframes have a divisions property. This is a tuple of
     # locations along the index where partitions start and stop. It looks like
     # this: (0, 10, 20, 29) for a dataframe with 3 divisions and 30 elements.
@@ -420,16 +440,28 @@
     result = result.rio.write_nodata(fill)
     return result
 
 
 def _geoms_to_raster_mask(xc, yc, geoms, all_touched=True, block_info=None):
     xc = xc.ravel()
     yc = yc.ravel()
-    # Convert geoms into a boolean (0/1) array using xc and yc for gridding.
     shape = (yc.size, xc.size)
+    cell_size = max(np.diff(xc).max(), np.diff(yc).max())
+    chunk_bbox = shapely.geometry.box(
+        xc.min(), yc.min(), xc.max(), yc.max()
+    ).buffer(cell_size)
+    geoms_bbox = shapely.geometry.box(*geoms.total_bounds)
+    if not shapely.intersects(chunk_bbox, geoms_bbox):
+        return np.zeros(shape, dtype="uint8")
+
+    geoms = geoms.clip(chunk_bbox)
+    if not len(geoms):
+        return np.zeros(shape, dtype="uint8")
+
+    # Convert geoms into a boolean (0/1) array using xc and yc for gridding.
     transform = xr.DataArray(
         da.zeros(shape), coords=(yc, xc), dims=("y", "x")
     ).rio.transform()
     # Use a MemoryFile to avoid writing to disk
     with rio.io.MemoryFile() as memfile, rio.open(
         memfile,
         mode="w+",
@@ -458,24 +490,100 @@
             yc,
             geoms=part,
             all_touched=all_touched,
             chunks=like.data.chunks[1:],
             meta=np.array((), dtype=I8),
         )
         parts.append(data)
-    data = da.stack(parts, axis=0).max(axis=0, keepdims=True)
+    data = da.stack(parts, axis=0).any(axis=0, keepdims=True).astype("uint8")
     x = like.x
     y = like.y
     xrs = xr.DataArray(data, coords=([1], y, x), dims=like.xdata.dims)
     if like.crs is not None:
         xrs = xrs.rio.write_crs(like.crs)
     xrs = xrs.rio.write_nodata(0)
     return xrs
 
 
+def rasterize(gdf, like, field=None, all_touched=True):
+    """Convert vector data to a raster.
+
+    Parameters
+    ----------
+    like : Raster
+        A to use for grid and CRS information. The resulting raster will be
+        on the same grid as `like`.
+    field : str, optional
+        The name of a field to use for fill values when rasterizing the
+        vector features.
+    all_touched : bool, optional
+        If ``True``, grid cells that the vector touches will be burned in.
+        If False, only cells with a center point inside of the vector
+        perimeter will be burned in.
+
+    Returns
+    -------
+    Raster
+        The resulting raster. The result will have a single band. Each
+        vector shape is assigned a 1-based integer value equal to its order
+        in the original vector collection. This integer value is what is
+        burned in at the corresponding grid cells. The dtype of the result
+        will be the minimum, unsigned integer type that can fit the ID
+        values. The null value is 0.
+
+    """
+    like = get_raster(like)
+    if field is not None:
+        if not is_str(field):
+            raise TypeError("Field must be a string")
+        if field not in gdf:
+            raise ValueError(f"Invalid field name: {repr(field)}")
+        dtype = gdf.dtypes.to_dict()[field]
+        if not is_int(dtype) and not is_float(dtype):
+            raise ValueError("The specified field must be a scalar data type")
+
+    xrs = _vector_to_raster_dask(
+        gdf.to_crs(like.crs),
+        gdf.size,
+        xlike=like.xdata,
+        field=field,
+        all_touched=all_touched,
+    )
+    return Raster(xrs)
+
+
+def rasterize_mask(gdf, like, all_touched=True):
+    """Convert vector data to a raster mask.
+
+    Parameters
+    ----------
+    like : Raster
+        A to use for grid and CRS information. The resulting raster will be
+        on the same grid as `like`.
+    all_touched : bool, optional
+        If ``True``, grid cells that the vector touches will be burned in.
+        If False, only cells with a center point inside of the vector
+        perimeter will be burned in.
+
+    Returns
+    -------
+    Raster
+        The resulting raster. The result will have a single band. All cells
+        that fall under the vector data are masked with ``1``. The null
+        value is 0.
+
+    """
+    like = get_raster(like)
+
+    xrs = _vector_to_raster_mask(
+        gdf.to_crs(like.crs).geometry, like, all_touched=all_touched
+    )
+    return Raster(xrs)
+
+
 def _normalize_geo_data(geo):
     if not _is_series(geo) and not _is_frame(geo):
         raise TypeError(
             "Invalid data type. Must be some type GeoDataFrame or"
             f" GeoSeries. Got {type(geo)}."
         )
     if _is_series(geo):
```

### Comparing `raster-tools-0.1.3/raster_tools/zonal.py` & `raster-tools-0.1.4/raster_tools/zonal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/raster_tools.egg-info/PKG-INFO` & `raster-tools-0.1.4/raster_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster-tools
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools for processing geospatial data
 Home-page: https://github.com/UM-RMRS/raster_tools
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/UM-RMRS/raster_tools/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `raster-tools-0.1.3/raster_tools.egg-info/SOURCES.txt` & `raster-tools-0.1.4/raster_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/setup.py` & `raster-tools-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/tests/test_clipping.py` & `raster-tools-0.1.4/tests/test_clipping.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/tests/test_distance.py` & `raster-tools-0.1.4/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/tests/test_distance__heap.py` & `raster-tools-0.1.4/tests/test_distance__heap.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/tests/test_distance_proximity.py` & `raster-tools-0.1.4/tests/test_distance_proximity.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/tests/test_focal.py` & `raster-tools-0.1.4/tests/test_focal.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/tests/test_general.py` & `raster-tools-0.1.4/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/tests/test_line_stats.py` & `raster-tools-0.1.4/tests/test_line_stats.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/tests/test_raster.py` & `raster-tools-0.1.4/tests/test_raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+# isort: off
+# TODO(pygeos): remove this once shapely is the default backend for geopandas.
+# Force raster_tools._compat to be loaded before geopandas when running tests
+import raster_tools  # noqa: F401
+
+# isort: on
+
 import operator
 import unittest
 
 import affine
 import dask
 import dask.array as da
 import numpy as np
@@ -877,23 +884,23 @@
 
 
 _NP_UFUNCS = list(
     filter(
         lambda x: isinstance(x, np.ufunc)
         # not valid for rasters
         and x not in (np.isnat, np.matmul),
-        map(lambda x: getattr(np, x), dir(np)),
+        map(lambda x: getattr(np, x), sorted(dir(np))),
     )
 )
 _NP_UFUNCS_NIN_SINGLE = list(filter(lambda x: x.nin == 1, _NP_UFUNCS))
 _NP_UFUNCS_NIN_MULT = list(filter(lambda x: x.nin > 1, _NP_UFUNCS))
-_UNSUPPORED_UFUNCS = frozenset((np.isnat, np.matmul))
+_UNSUPPORED_UFUNCS = [np.isnat, np.matmul]
 
 
-@pytest.mark.parametrize("ufunc", list(_UNSUPPORED_UFUNCS))
+@pytest.mark.parametrize("ufunc", _UNSUPPORED_UFUNCS)
 def test_ufuncs_unsupported(ufunc):
     rs = Raster(np.arange(4 * 5 * 5).reshape((4, 5, 5)))
     with pytest.raises(TypeError):
         args = [rs for i in range(ufunc.nin)]
         ufunc(*args)
 
 
@@ -1093,14 +1100,52 @@
                 assert_valid_raster(r)
                 t[mask] = get_default_null_value(t.dtype)
                 assert r.crs == rs.crs
                 assert np.allclose(r, t, equal_nan=True)
                 assert np.allclose(r._ds.mask, mask, equal_nan=True)
 
 
+def test_ufunc_different_masks():
+    r1 = arange_raster((3, 3)).set_null_value(0)
+    r1.mask[..., :2, :] = True
+    r2 = arange_raster((3, 3)).set_null_value(0)
+    r2.mask[..., :, :2] = True
+    r1_mask = np.array(
+        [
+            [
+                [1, 1, 1],
+                [1, 1, 1],
+                [0, 0, 0],
+            ]
+        ]
+    )
+    r2_mask = np.array(
+        [
+            [
+                [1, 1, 0],
+                [1, 1, 0],
+                [1, 1, 0],
+            ]
+        ]
+    )
+    result_mask = r1_mask | r2_mask
+    assert np.allclose(r1.mask.compute(), r1_mask)
+    assert np.allclose(r2.mask.compute(), r2_mask)
+    assert np.allclose(
+        result_mask, np.array([[1, 1, 1], [1, 1, 1], [1, 1, 0]])
+    )
+
+    result = r1 * r2
+    # Make sure that there where no side effects on the input raster masks
+    assert np.allclose(r1.mask.compute(), r1_mask)
+    assert np.allclose(r2.mask.compute(), r2_mask)
+    result_data = np.where(result_mask, result.null_value, 64)
+    assert np.allclose(result, result_data)
+
+
 def test_invert():
     x = arange_nd((4, 5, 5))
     rs = Raster(x)
     rs._ds["raster"] = xr.where(
         (0 <= rs._ds.raster) & (rs._ds.raster < 10), 0, rs._ds.raster
     )
     rs = rs.set_null_value(0).set_crs("EPSG:3857")
```

### Comparing `raster-tools-0.1.3/tests/test_stat_common.py` & `raster-tools-0.1.4/tests/test_stat_common.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/tests/test_surface.py` & `raster-tools-0.1.4/tests/test_surface.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/tests/test_vector.py` & `raster-tools-0.1.4/tests/test_vector.py`

 * *Files identical despite different names*

### Comparing `raster-tools-0.1.3/tests/test_zonal.py` & `raster-tools-0.1.4/tests/test_zonal.py`

 * *Files identical despite different names*


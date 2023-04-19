# Comparing `tmp/momlevel-0.0.7.tar.gz` & `tmp/momlevel-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momlevel-0.0.7.tar", last modified: Wed Jan 25 00:25:20 2023, max compression
+gzip compressed data, was "momlevel-0.0.8.tar", last modified: Wed Apr 19 20:24:22 2023, max compression
```

## Comparing `momlevel-0.0.7.tar` & `momlevel-0.0.8.tar`

### file list

```diff
@@ -1,42 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 00:25:20.821879 momlevel-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-01-25 00:25:07.000000 momlevel-0.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-01-25 00:25:20.821879 momlevel-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-25 00:25:07.000000 momlevel-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-01-25 00:25:07.000000 momlevel-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 00:25:20.821879 momlevel-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 00:25:20.789879 momlevel-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 00:25:20.797879 momlevel-0.0.7/src/momlevel/
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24149 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/derived.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/dynamic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 00:25:20.797879 momlevel-0.0.7/src/momlevel/eos/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/eos/wright.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 00:25:20.821879 momlevel-0.0.7/src/momlevel/resources/
--rw-r--r--   0 runner    (1001) docker     (123) 18167522 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/resources/CM4_historical.nc
--rw-r--r--   0 runner    (1001) docker     (123)   801596 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/resources/NWA12_grid_dataframe.csv
--rw-r--r--   0 runner    (1001) docker     (123)  3377003 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/resources/NWA12_sample_grid_data.nc
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/resources/geolocate_points_reference.csv
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/resources/global_tide_gauges.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/resources/us_tide_gauges.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 00:25:20.821879 momlevel-0.0.7/src/momlevel/spice/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/spice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/spice/flament.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/steric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 00:25:20.821879 momlevel-0.0.7/src/momlevel/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/test_data/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 00:25:20.821879 momlevel-0.0.7/src/momlevel/test_data/tripolar/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/test_data/tripolar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/test_data/tripolar/horizontal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/test_data/tripolar/vertical.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/tidegauge.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/trend.py
--rw-r--r--   0 runner    (1001) docker     (123)    23591 2023-01-25 00:25:07.000000 momlevel-0.0.7/src/momlevel/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 00:25:20.797879 momlevel-0.0.7/src/momlevel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-01-25 00:25:20.000000 momlevel-0.0.7/src/momlevel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-01-25 00:25:20.000000 momlevel-0.0.7/src/momlevel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 00:25:20.000000 momlevel-0.0.7/src/momlevel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-25 00:25:20.000000 momlevel-0.0.7/src/momlevel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-25 00:25:20.000000 momlevel-0.0.7/src/momlevel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.621268 momlevel-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-19 20:24:10.000000 momlevel-0.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-19 20:24:22.621268 momlevel-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-19 20:24:10.000000 momlevel-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-04-19 20:24:10.000000 momlevel-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 20:24:22.621268 momlevel-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.597268 momlevel-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.597268 momlevel-0.0.8/src/momlevel/
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-19 20:24:10.000000 momlevel-0.0.8/src/momlevel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24149 2023-04-19 20:24:10.000000 momlevel-0.0.8/src/momlevel/derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-04-19 20:24:10.000000 momlevel-0.0.8/src/momlevel/dynamic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.597268 momlevel-0.0.8/src/momlevel/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-19 20:24:10.000000 momlevel-0.0.8/src/momlevel/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-19 20:24:10.000000 momlevel-0.0.8/src/momlevel/eos/wright.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-19 20:24:10.000000 momlevel-0.0.8/src/momlevel/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.621268 momlevel-0.0.8/src/momlevel/resources/
+-rw-r--r--   0 runner    (1001) docker     (123) 18167522 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/resources/CM4_historical.nc
+-rw-r--r--   0 runner    (1001) docker     (123)   801596 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/resources/NWA12_grid_dataframe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)  3377003 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/resources/NWA12_sample_grid_data.nc
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/resources/geolocate_points_reference.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/resources/global_tide_gauges.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/resources/us_tide_gauges.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.621268 momlevel-0.0.8/src/momlevel/spice/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/spice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/spice/flament.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/steric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.621268 momlevel-0.0.8/src/momlevel/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)    10214 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/test_data/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.621268 momlevel-0.0.8/src/momlevel/test_data/tripolar/
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/test_data/tripolar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/test_data/tripolar/horizontal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/test_data/tripolar/vertical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/tidegauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/trend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23591 2023-04-19 20:24:11.000000 momlevel-0.0.8/src/momlevel/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.597268 momlevel-0.0.8/src/momlevel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-19 20:24:22.000000 momlevel-0.0.8/src/momlevel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-19 20:24:22.000000 momlevel-0.0.8/src/momlevel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:24:22.000000 momlevel-0.0.8/src/momlevel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-19 20:24:22.000000 momlevel-0.0.8/src/momlevel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 20:24:22.000000 momlevel-0.0.8/src/momlevel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:24:22.621268 momlevel-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4304 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_derived.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_flament.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_steric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_testdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_tidegauge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_trend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-19 20:24:11.000000 momlevel-0.0.8/tests/test_wright.py
```

### Comparing `momlevel-0.0.7/LICENSE.txt` & `momlevel-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/PKG-INFO` & `momlevel-0.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momlevel
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tools to diagnose sea level in the MOM Ocean Model
 Author-email: John Krasting <john.krasting@noaa.gov>
 License: Software code created by U.S. Government employees is not subject to copyright in the United States (17 U.S.C. §105).
         The United States/Department of Commerce reserve all rights to seek and obtain copyright protection in countries
         otherthan the United States for Software authored in its entirety by the Department of Commerce. To this end, the
         Department of Commerce hereby grants to Recipient a royalty-free, nonexclusive license to use, copy, and create 
         derivative works of the Software outside of the United States.”
```

### Comparing `momlevel-0.0.7/README.md` & `momlevel-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/pyproject.toml` & `momlevel-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/__init__.py` & `momlevel-0.0.8/src/momlevel/__init__.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/derived.py` & `momlevel-0.0.8/src/momlevel/derived.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/dynamic.py` & `momlevel-0.0.8/src/momlevel/dynamic.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/eos/wright.py` & `momlevel-0.0.8/src/momlevel/eos/wright.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/reference.py` & `momlevel-0.0.8/src/momlevel/reference.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/resources/CM4_historical.nc` & `momlevel-0.0.8/src/momlevel/resources/CM4_historical.nc`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/resources/NWA12_grid_dataframe.csv` & `momlevel-0.0.8/src/momlevel/resources/NWA12_grid_dataframe.csv`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/resources/NWA12_sample_grid_data.nc` & `momlevel-0.0.8/src/momlevel/resources/NWA12_sample_grid_data.nc`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/resources/geolocate_points_reference.csv` & `momlevel-0.0.8/src/momlevel/resources/geolocate_points_reference.csv`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/resources/global_tide_gauges.csv` & `momlevel-0.0.8/src/momlevel/resources/global_tide_gauges.csv`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/resources/us_tide_gauges.csv` & `momlevel-0.0.8/src/momlevel/resources/us_tide_gauges.csv`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/spice/flament.py` & `momlevel-0.0.8/src/momlevel/spice/flament.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/steric.py` & `momlevel-0.0.8/src/momlevel/steric.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/test_data/__init__.py` & `momlevel-0.0.8/src/momlevel/test_data/__init__.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/test_data/time.py` & `momlevel-0.0.8/src/momlevel/test_data/time.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/test_data/tripolar/horizontal.py` & `momlevel-0.0.8/src/momlevel/test_data/tripolar/horizontal.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/test_data/tripolar/vertical.py` & `momlevel-0.0.8/src/momlevel/test_data/tripolar/vertical.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/tidegauge.py` & `momlevel-0.0.8/src/momlevel/tidegauge.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel/trend.py` & `momlevel-0.0.8/src/momlevel/trend.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """ trend.py - utilities for working with trends """
 
 import warnings
-
+import numpy as np
 import xarray as xr
 
 __all__ = [
     "broadcast_trend",
     "calc_linear_trend",
     "linear_detrend",
     "time_conversion_factor",
+    "seasonal_model",
 ]
 
 
 def broadcast_trend(slope, dim_arr):
     """Function to broadcast a trend along a dimension
 
     This function broadcasts a trend against a dimension to obtain a
@@ -46,15 +47,14 @@
     # Get the dimension name for reuse
     dim_name = dim_arr.dims[0]
 
     # Determine if we have time trend. If so, check the units and convert
     # to nanoseconds if necessary
     time_indexes = [xr.coding.cftimeindex.CFTimeIndex]
     if any([isinstance(dim_arr.indexes[dim_name], x) for x in time_indexes]):
-
         # Flag to throw default behavior warning
         warn_time_units = False
 
         # If slope/trend array has a units attribute, try to do something
         if "units" in slope.attrs.keys():
             units = slope.attrs["units"].split(" ")
             units = [x.replace("-1", "") for x in units if "-1" in x]
@@ -309,15 +309,14 @@
 
     # case 1: input object is xarray.DataArray
     if isinstance(xobj, xr.DataArray):
         result = _detrend_array(xobj, dim=dim, order=order, mode=mode)
 
     # case 2: input object is xarray.Dataset
     elif isinstance(xobj, xr.Dataset):
-
         varlist = list(xobj.keys())
 
         # quick sanity check
         questionable_vars = ["time_bnds", "average_T1", "average_T2", "average_DT"]
         if any(var in varlist for var in questionable_vars):
             warnings.warn(
                 "Incompatible variable detected. "
@@ -338,7 +337,111 @@
         # convert dict back to xarray.Dataset
         result = xr.Dataset(result)
 
     else:
         raise TypeError("Input must be xarray.DataArray or xarray.Dataset")
 
     return result
+
+
+def seasonal_model(da_timeseries, tcoord="time", return_model=False):
+    """Function to calculate a seasonal cycle in a time series
+    This function creates a modelled time series that includes
+    a linear trend and annual and semi-annual harmonics
+
+    f(time) = b + m * time + c1 * sin(2*pi*time/year) + ...
+        c2 * cos(2*pi*time/year) + c3 * sin(4*pi*time/year) + ...
+        c4 * cos(4*pi*time/year) + residual
+
+    Parameters
+    ----------
+    da_timeseries : xarray.core.dataarray.DataArray
+        A time series in a DataArray format, which can be of
+        arbitrary dimensionality
+    tcoord : str, optional
+        Name of the time coordinate, if present, by default "time"
+    Returns
+    -------
+    residuals : xarray.core.dataarray.DataArray
+        Residuals from modelled fit
+    seasonal_model : xarray.core.dataarray.DataArray
+        Modelled seasonal cycle of time series (returned only if return_model=True)
+    """
+    # PREPROCESSING
+    # Here we find the non-time coordinates for our dataset and create a hashable
+    # so that the model can be expanded to an arbitrary number of dimensions
+    # If coordinates are empty we drop them
+    da_timeseries = da_timeseries.reset_coords(drop=True)
+    coords = [x for x in da_timeseries.coords if x != tcoord]
+    coords = tuple(coords)
+
+    coords_dict = {}
+    for coord_name in coords:
+        coords_dict[coord_name] = da_timeseries[f"{coord_name}"]
+    hashable_coords = {key: tuple(val.values) for key, val in coords_dict.items()}
+
+    # From here we use the same code provided by John, extended to multiple dimensions
+    time_dec = (
+        da_timeseries[tcoord].dt.year
+        + (da_timeseries[tcoord].dt.dayofyear - 1 + da_timeseries[tcoord].dt.hour / 24)
+        / 365
+    )
+
+    model = np.array(
+        [np.ones(len(time_dec))]
+        + [time_dec - np.mean(time_dec)]
+        + [np.sin(2 * np.pi * time_dec)]
+        + [np.cos(2 * np.pi * time_dec)]
+        + [np.sin(4 * np.pi * time_dec)]
+        + [np.cos(4 * np.pi * time_dec)]
+    )
+
+    pmodel = np.linalg.pinv(model)
+
+    model_da = xr.DataArray(
+        model,
+        dims=["coeff", "time"],
+        coords={"coeff": np.arange(1, 7, 1), "time": da_timeseries[tcoord]},
+    )
+    model_da = model_da.expand_dims(dim=hashable_coords)
+
+    pmodel_da = xr.DataArray(
+        pmodel,
+        dims=["time", "coeff"],
+        coords={"coeff": np.arange(1, 7, 1), "time": da_timeseries[tcoord]},
+    )
+    pmodel_da = pmodel_da.expand_dims(dim=hashable_coords)
+
+    mcoeff = pmodel_da.dot(da_timeseries, dims="time")
+
+    smodel = model_da.dot(mcoeff, dims="coeff")
+    residuals = da_timeseries - smodel
+
+    if "standard_name" in da_timeseries.attrs.keys():
+        _standard_name_m = da_timeseries.attrs["standard_name"] + "_smodel"
+        _standard_name_r = da_timeseries.attrs["standard_name"] + "_sresid"
+    else:
+        _standard_name_m = "smodel"
+        _standard_name_r = "sresid"
+
+    if "long_name" in da_timeseries.attrs.keys():
+        _long_name_m = "Seasonal model, " + da_timeseries.attrs["long_name"]
+        _long_name_r = "Seasonal residuals, " + da_timeseries.attrs["long_name"]
+    else:
+        _long_name_m = "Seasonal model"
+        _long_name_r = "Seasonal residuals"
+
+    if "units" in da_timeseries.attrs.keys():
+        _units = da_timeseries.attrs["units"]
+    else:
+        _units = ""
+
+    smodel.attrs["standard_name"] = _standard_name_m
+    smodel.attrs["long_name"] = _long_name_m
+    smodel.attrs["units"] = _units
+
+    residuals.attrs["standard_name"] = _standard_name_r
+    residuals.attrs["long_name"] = _long_name_r
+    residuals.attrs["units"] = _units
+    if return_model:
+        return smodel, residuals
+    return residuals
```

### Comparing `momlevel-0.0.7/src/momlevel/util.py` & `momlevel-0.0.8/src/momlevel/util.py`

 * *Files identical despite different names*

### Comparing `momlevel-0.0.7/src/momlevel.egg-info/PKG-INFO` & `momlevel-0.0.8/src/momlevel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: momlevel
-Version: 0.0.7
+Version: 0.0.8
 Summary: Tools to diagnose sea level in the MOM Ocean Model
 Author-email: John Krasting <john.krasting@noaa.gov>
 License: Software code created by U.S. Government employees is not subject to copyright in the United States (17 U.S.C. §105).
         The United States/Department of Commerce reserve all rights to seek and obtain copyright protection in countries
         otherthan the United States for Software authored in its entirety by the Department of Commerce. To this end, the
         Department of Commerce hereby grants to Recipient a royalty-free, nonexclusive license to use, copy, and create 
         derivative works of the Software outside of the United States.”
```


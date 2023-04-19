# Comparing `tmp/elwood-0.1.1-9-py2.py3-none-any.whl.zip` & `tmp/elwood-0.1.2-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,30 @@
-Zip file size: 50195 bytes, number of entries: 25
--rw-rw-r--  2.0 unx      126 b- defN 23-Feb-20 20:58 elwood/__init__.py
--rw-rw-r--  2.0 unx    17984 b- defN 23-Mar-20 16:57 elwood/cli.py
+Zip file size: 63120 bytes, number of entries: 28
+-rw-rw-r--  2.0 unx      126 b- defN 23-Apr-19 20:19 elwood/__init__.py
+-rw-rw-r--  2.0 unx    17988 b- defN 23-Apr-19 20:19 elwood/cli.py
 -rw-rw-r--  2.0 unx      409 b- defN 23-Feb-16 15:03 elwood/constants.py
 -rw-rw-r--  2.0 unx     3042 b- defN 23-Mar-20 16:57 elwood/download.py
--rw-rw-r--  2.0 unx    10799 b- defN 23-Mar-20 16:57 elwood/elwood.py
--rw-rw-r--  2.0 unx      689 b- defN 23-Feb-16 15:03 elwood/feature_scaling.py
+-rw-rw-r--  2.0 unx    11168 b- defN 23-Apr-19 20:19 elwood/elwood.py
+-rw-rw-r--  2.0 unx     4607 b- defN 23-Apr-19 20:19 elwood/feature_normalization.py
+-rw-rw-r--  2.0 unx      689 b- defN 23-Mar-31 16:42 elwood/feature_scaling.py
 -rw-rw-r--  2.0 unx     9756 b- defN 23-Mar-20 16:57 elwood/file_processor.py
 -rw-rw-r--  2.0 unx    12542 b- defN 23-Mar-20 16:57 elwood/geo_processor.py
 -rw-rw-r--  2.0 unx    24705 b- defN 23-Mar-20 16:57 elwood/normalizer.py
+-rw-rw-r--  2.0 unx    24707 b- defN 23-Apr-19 20:19 elwood/standardizer.py
 -rw-rw-r--  2.0 unx     2313 b- defN 23-Mar-20 16:57 elwood/time_helpers.py
 -rw-rw-r--  2.0 unx    11713 b- defN 23-Mar-20 16:57 elwood/time_processor.py
 -rw-rw-r--  2.0 unx     4602 b- defN 23-Feb-15 22:42 elwood/data/iso_lookup.csv
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-16 15:03 elwood/transformations/__init__.py
 -rw-rw-r--  2.0 unx     2007 b- defN 23-Mar-20 16:57 elwood/transformations/clipping.py
 -rw-rw-r--  2.0 unx      424 b- defN 23-Feb-16 15:03 elwood/transformations/geo_utils.py
--rw-rw-r--  2.0 unx     2236 b- defN 23-Mar-20 16:57 elwood/transformations/regridding.py
--rw-rw-r--  2.0 unx     1349 b- defN 23-Mar-23 17:58 elwood/transformations/scaling.py
+-rw-rw-r--  2.0 unx    16372 b- defN 23-Apr-19 20:19 elwood/transformations/outlier_scaling.py
+-rw-rw-r--  2.0 unx     2410 b- defN 23-Apr-19 20:19 elwood/transformations/regridding.py
+-rw-rw-r--  2.0 unx     1474 b- defN 23-Apr-19 20:19 elwood/transformations/scaling.py
 -rw-rw-r--  2.0 unx      141 b- defN 23-Feb-17 18:00 elwood/transformations/temporal_utils.py
--rw-rw-r--  2.0 unx      123 b- defN 23-Mar-23 18:00 elwood-0.1.1.dist-info/AUTHORS.md
--rw-rw-r--  2.0 unx    35149 b- defN 23-Mar-23 18:00 elwood-0.1.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4943 b- defN 23-Mar-23 18:00 elwood-0.1.1.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-Mar-23 18:00 elwood-0.1.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx       43 b- defN 23-Mar-23 18:00 elwood-0.1.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        7 b- defN 23-Mar-23 18:00 elwood-0.1.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     2048 b- defN 23-Mar-23 18:00 elwood-0.1.1.dist-info/RECORD
-25 files, 147260 bytes uncompressed, 46901 bytes compressed:  68.2%
+-rw-rw-r--  2.0 unx      123 b- defN 23-Apr-19 20:19 elwood-0.1.2.dist-info/AUTHORS.md
+-rw-rw-r--  2.0 unx    35149 b- defN 23-Apr-19 20:19 elwood-0.1.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4943 b- defN 23-Apr-19 20:19 elwood-0.1.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-Apr-19 20:19 elwood-0.1.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       43 b- defN 23-Apr-19 20:19 elwood-0.1.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        7 b- defN 23-Apr-19 20:19 elwood-0.1.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2315 b- defN 23-Apr-19 20:19 elwood-0.1.2.dist-info/RECORD
+28 files, 193885 bytes uncompressed, 59410 bytes compressed:  69.4%
```

## zipnote {}

```diff
@@ -9,26 +9,32 @@
 
 Filename: elwood/download.py
 Comment: 
 
 Filename: elwood/elwood.py
 Comment: 
 
+Filename: elwood/feature_normalization.py
+Comment: 
+
 Filename: elwood/feature_scaling.py
 Comment: 
 
 Filename: elwood/file_processor.py
 Comment: 
 
 Filename: elwood/geo_processor.py
 Comment: 
 
 Filename: elwood/normalizer.py
 Comment: 
 
+Filename: elwood/standardizer.py
+Comment: 
+
 Filename: elwood/time_helpers.py
 Comment: 
 
 Filename: elwood/time_processor.py
 Comment: 
 
 Filename: elwood/data/iso_lookup.csv
@@ -39,38 +45,41 @@
 
 Filename: elwood/transformations/clipping.py
 Comment: 
 
 Filename: elwood/transformations/geo_utils.py
 Comment: 
 
+Filename: elwood/transformations/outlier_scaling.py
+Comment: 
+
 Filename: elwood/transformations/regridding.py
 Comment: 
 
 Filename: elwood/transformations/scaling.py
 Comment: 
 
 Filename: elwood/transformations/temporal_utils.py
 Comment: 
 
-Filename: elwood-0.1.1.dist-info/AUTHORS.md
+Filename: elwood-0.1.2.dist-info/AUTHORS.md
 Comment: 
 
-Filename: elwood-0.1.1.dist-info/LICENSE
+Filename: elwood-0.1.2.dist-info/LICENSE
 Comment: 
 
-Filename: elwood-0.1.1.dist-info/METADATA
+Filename: elwood-0.1.2.dist-info/METADATA
 Comment: 
 
-Filename: elwood-0.1.1.dist-info/WHEEL
+Filename: elwood-0.1.2.dist-info/WHEEL
 Comment: 
 
-Filename: elwood-0.1.1.dist-info/entry_points.txt
+Filename: elwood-0.1.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: elwood-0.1.1.dist-info/top_level.txt
+Filename: elwood-0.1.2.dist-info/top_level.txt
 Comment: 
 
-Filename: elwood-0.1.1.dist-info/RECORD
+Filename: elwood-0.1.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## elwood/__init__.py

```diff
@@ -1,5 +1,5 @@
 """Top-level package for elwood."""
 
 __author__ = """Brandon Rose"""
 __email__ = "brandon@jataware.com"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

## elwood/cli.py

```diff
@@ -1,14 +1,14 @@
 import os
 
 import click
 import pandas as pd
 
 from .download import download_and_clean
-from .elwood import normalizer, optimize_df_types, mixdata
+from .elwood import standardizer, optimize_df_types, mixdata
 from .file_processor import netcdf2df_processor, raster2df_processor
 from .geo_processor import geocode
 
 from glob import glob
 import numpy as np
 
 import json
@@ -116,15 +116,15 @@
     # Iterate chunk tmp files and normalize each loaded df.
     for i in range(1, chunks + 1):
         read_filename = f"{DATA_TEMP_FILENAME}.{i}.pkl"
         df_temp = pd.read_pickle(read_filename)
 
         ## Run normalizer.
         norm_start_time = timeit.default_timer()
-        norm, result_dict = normalizer(
+        norm, result_dict = standardizer(
             df_temp, mapper, geo, gadm=gadm, df_geocode=df_geocode
         )
 
         # Normalizer will add NaN for missing values, e.g. when appending
         # dataframes with different columns. GADM will return None when geocoding
         # but not finding the entity (e.g. admin3 for United States).
         # Replace None with NaN for consistency.
```

## elwood/elwood.py

```diff
@@ -10,16 +10,16 @@
 
 from . import constants
 from .file_processor import (
     process_file_by_filetype,
     raster2df_processor,
     netcdf2df_processor,
 )
-from .normalizer import normalizer
-from .feature_scaling import scale_dataframe
+from .standardizer import standardizer
+from .feature_normalization import zero_to_one_normalization, robust_normalization
 from .transformations.clipping import construct_multipolygon, clip_dataframe, clip_time
 from .transformations.scaling import scale_time
 from .transformations.regridding import regrid_dataframe
 from .transformations.geo_utils import calculate_boundary_box
 from .transformations.temporal_utils import calculate_temporal_boundary
 
 if not sys.warnoptions:
@@ -75,15 +75,15 @@
     ## To speed up normalize(), reduce the memory size of the dataframe by:
     # 1. Optimize the dataframe types.
     # 2. Reset the index so it is a RangeIndex instead of Int64Index.
     df = optimize_df_types(df)
     df.reset_index(inplace=True, drop=True)
 
     ## Run normalizer.
-    norm, renamed_col_dict = normalizer(df, mapper, admin, gadm=gadm)
+    norm, renamed_col_dict = standardizer(df, mapper, admin, gadm=gadm)
 
     # Normalizer will add NaN for missing values, e.g. when appending
     # dataframes with different columns. GADM will return None when geocoding
     # but not finding the entity (e.g. admin3 for United States).
     # Replace None with NaN for consistency.
     norm.fillna(value=np.nan, inplace=True)
 
@@ -133,21 +133,31 @@
     Args:
         dataframe (pandas.Dataframe): A pandas dataframe with a "feature" and "value" column.
         Will scale numerical values in the "value" column from 0 to 1.
 
     Returns:
         pandas.Dataframe: Returns a pandas Dataframe with numerical features scaled from 0 to 1.
     """
-    df = scale_dataframe(dataframe)
+    df = zero_to_one_normalization(dataframe)
 
     if output_file:
         df.to_parquet(f"{output_file}_normalized.parquet.gzip", compression="gzip")
     return df
 
 
+def normalize_features_robust(dataframe, output_file: str = None):
+    df = robust_normalization(dataframe, method="min_max")
+
+    if output_file:
+        df.to_parquet(
+            f"{output_file}_normalized_robust.parquet.gzip", compression="gzip"
+        )
+    return df
+
+
 def clip_geo(dataframe, geo_columns, polygons_list):
     """Clips data based on geographical shape(s) or shapefile (NOT IMPLEMENTED).
 
     Args:
         dataframe (pandas.Dataframe): A pandas dataframe containing geographical data.
         geo_columns (list): A list containing the two column names for the lat/lon columns in the dataframe.
         polygons_list (list[list[obj]]): A list containing lists of objects that represent polygon shapes to clip to.
@@ -175,15 +185,15 @@
 
     return clip_time(
         dataframe=dataframe, time_column=time_column, time_ranges=time_ranges
     )
 
 
 def rescale_dataframe_time(
-    dataframe, time_column, time_bucket, aggregation_function_list
+    dataframe, time_column, time_bucket, aggregation_functions, geo_columns=None
 ):
     """Rescales a dataframes time periodicity using aggregation functions.
 
     Args:
         dataframe (pandas.Dataframe): A dataframe containing a column of time values to be rescaled
         time_column (string): Name of target time column
         time_bucket (DateOffset, Timedelta or str): Some time bucketing rule to lump the time in to. ex. 'M', 'A', '2H'
@@ -192,15 +202,16 @@
     Returns:
         _type_: _description_
     """
     return scale_time(
         dataframe=dataframe,
         time_column=time_column,
         time_bucket=time_bucket,
-        aggregation_function_list=aggregation_function_list,
+        aggregation_functions=aggregation_functions,
+        geo_columns=geo_columns,
     )
 
 
 def regrid_dataframe_geo(dataframe, geo_columns, time_column, scale_multi, scale=None):
     """Regrids a dataframe with detectable geo-resolution
 
     Args:
```

## elwood/transformations/regridding.py

```diff
@@ -4,22 +4,24 @@
 
 
 def regrid_dataframe(dataframe, geo_columns, time_column, scale_multi, scale=None):
     """Uses xarray interpolation to regrid geography in a dataframe.
 
     Args:
         dataframe (pandas.Dataframe): Dataframe of a dataset that has detectable gridden geographical resolution ie. points that represent 1sqkm areas
-        geo_columns (List[str]): The geo_columns for the latitude and longitude pairs.
+        geo_columns (List[str]): A list containing the geo_columns for the latitude and longitude pairs.
+        time_column (List[str]): A list containing the name of the datetime column(s) in the dataset.
         scale_multi (int): The number by which to divide to geographical scale to regrid larger.
 
     Returns:
         pandas.Dataframe: Dataframe with geographical extend regridded to
     """
 
-    geo_columns = geo_columns.extend(time_column)
+    geo_columns.extend(time_column)
+    ds = None
 
     try:
 
         ds = xarray.Dataset.from_dataframe(dataframe.set_index(geo_columns))
 
     except KeyError as error:
         print(error)
@@ -48,17 +50,18 @@
         round(ds.dims[geo_columns[1]] * multiplier),
     )
 
     interpolation = {geo_columns[0]: new_0, geo_columns[1]: new_1}
 
     ds2 = ds.interp(**interpolation)
 
-    p_dataframe = ds2.to_dataframe()
+    final_dataframe = ds2.to_dataframe()
+    final_dataframe.reset_index(inplace=True)
 
-    return p_dataframe
+    return final_dataframe
 
 
 def getScale(lat0, lon0, lat1, lon1):
     """
     Description
     -----------
     Return an estimation of the scale in km of a netcdf dataset.
```

## elwood/transformations/scaling.py

```diff
@@ -1,34 +1,33 @@
 import pandas
 
 
 def scale_time(
-    dataframe, time_column, time_bucket, aggregation_function_list, geo_columns=None
+    dataframe, time_column, time_bucket, aggregation_functions, geo_columns=None
 ):
     """Scales timestamp data in a dataframe to a less granular time frequency
 
     Args:
         dataframe (pandas.Dataframe): pandas dataframe with a timestamp field.
         time_column (string): Name of the time column to scale in the dataframe.
         time_bucket (DateOffset, Timedelta or str): The offset string or object representing target conversion. ex. "2H", "M"
-        aggregation_function (List[string]): A list of aggregation functions like sum, average, median, mean, mode, etc. Example: ['sum'], or ['min', 'max', 'sum']
+        aggregation_functions (List[string] or Dict{str:str}): A list containing one aggregation function, or a Dict containing column
+            names and aggregation functions like sum, average, median, mean, mode, etc. Example: ['sum'], or {'temp': 'min', 'rainfall': 'max', 'visitors': 'sum'}
         geo_columns (List[string]): A list of the geographical columns that should not be modified by the transformation.
     """
 
     dataframe[time_column] = pandas.to_datetime(dataframe[time_column])
 
     if geo_columns:
         dataframe = dataframe.set_index(geo_columns)
 
         dataframe = dataframe.groupby(geo_columns)
 
-    # dataframe.set_index(time_column).resample(time_bucket).agg(
-    # aggregation_function_list
-    # )
-    scaled_frame = dataframe.resample(time_bucket, on=time_column).agg(
-        aggregation_function_list[0]
-    )
+    aggregator = aggregation_functions
+    if isinstance(aggregation_functions, list):
+        aggregator = aggregation_functions[0]
+    scaled_frame = dataframe.resample(time_bucket, on=time_column).agg(aggregator)
 
     # scaled_frame.columns = scaled_frame.columns.get_level_values(0)
     scaled_frame.reset_index(inplace=True)
 
     return scaled_frame
```

## Comparing `elwood-0.1.1.dist-info/LICENSE` & `elwood-0.1.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `elwood-0.1.1.dist-info/METADATA` & `elwood-0.1.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elwood
-Version: 0.1.1
+Version: 0.1.2
 Summary: An open source dataset transformation, standardization, and normalization python library.
 Home-page: https://github.com/jataware/elwood
 Author: Brandon Rose, Powell Fendley
 Author-email: info@jataware.com
 License: MIT license
 Keywords: elwood
 Platform: UNKNOWN
```

## Comparing `elwood-0.1.1.dist-info/RECORD` & `elwood-0.1.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-elwood/__init__.py,sha256=W-7EbE6BmNGeVmF4pGHaDJs2oEIIwiNP-gI34xwR2i8,126
-elwood/cli.py,sha256=lFuXxs0rgCyYqCofFpeau6YB43a4EkkP2RGR_SSYPCQ,17984
+elwood/__init__.py,sha256=Dq2HwvPsxX7-Y_TV0v4Us0Icx86C4ODbIZ_nPh8k7HM,126
+elwood/cli.py,sha256=M4-2TU-q9tyBDSlj9HN4w2_2YcROr2JMqYj5nUySe6o,17988
 elwood/constants.py,sha256=ZthYZ6NWPGrBpsHuVgYTY4CfGW5TDY7woUiuuGVNAvw,409
 elwood/download.py,sha256=E0oI7P3rR5nt7TYN00TnJmtgCalGiuJS1TPn4F4qX3A,3042
-elwood/elwood.py,sha256=jjXJQ9F-ySqkdzKpLaSjkb4GnYMgrjTAme2dfEs1kKE,10799
+elwood/elwood.py,sha256=ZqtD5C6Xlcg0S6ulUwpEC8aST4ePyyriZeGdV7XrZBQ,11168
+elwood/feature_normalization.py,sha256=-vAFEqEI5xt3aqrv-gLlZxjENlIW3aI44riqmu-n6uA,4607
 elwood/feature_scaling.py,sha256=gZaWWJ9n69tMw8fX7AAd5-FLc4uyYYaK-2tsQDkxYiI,689
 elwood/file_processor.py,sha256=V9FNr5WX11LCGQTx4zBYoXMKjZd8hAAiYmH7xS6Re3s,9756
 elwood/geo_processor.py,sha256=a0P90yBmrNwAq_JiDZbyyW8pihVjNUCO2C4kpapf62s,12542
 elwood/normalizer.py,sha256=cFM4B4-J5tg0aykdm_lSlyR5BQDKbB2rMrDsxsEg5JQ,24705
+elwood/standardizer.py,sha256=2MjtmPNMzgAwRGic9rErlTZbYk571wSsVt-JkMhTyDo,24707
 elwood/time_helpers.py,sha256=MX55zyBRggJ-lcVAhDRM-1HrfiaBeQXFt6D86dz0v9c,2313
 elwood/time_processor.py,sha256=_cLtRBX478CewVOMtSJjWhRx_S4z0TzMgDqyGs8Y8aY,11713
 elwood/data/iso_lookup.csv,sha256=nPPErF9kP2fU_s4IkldxgyUc5NnbYMbePrDYLQAoHSQ,4602
 elwood/transformations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 elwood/transformations/clipping.py,sha256=6LKx8qap0xiWiDgm2Hb7_aavxCVUcpAYEc1EOFvyfx8,2007
 elwood/transformations/geo_utils.py,sha256=p_c14Gy3k5dC8XWcPfeWldwDyhufjBWNptCyUUOeaD4,424
-elwood/transformations/regridding.py,sha256=rc8r6xAJoBcW7uIqktbkwYbHhps7K7XRSK22ghqRjNg,2236
-elwood/transformations/scaling.py,sha256=3PpgJ2I6Gc4M94GaqqY3XokoYOOC5Cvvm5h186cXT8c,1349
+elwood/transformations/outlier_scaling.py,sha256=O_K57Xx-eqOVC2MHr1h3E-QpyK70QRumPVmoPLtMtjI,16372
+elwood/transformations/regridding.py,sha256=N2Mo1MKJ2OrzfPr-Ac3l-S2yIiWINn-W5SsvPFsKKOo,2410
+elwood/transformations/scaling.py,sha256=skRvRSuudgViBDo3HmAuOh6G27pUmTwILCd0gelk7j4,1474
 elwood/transformations/temporal_utils.py,sha256=CxT29J3GfK4h6onFlNphojBP_IA9nL5G3c1r9Vh8QDE,141
-elwood-0.1.1.dist-info/AUTHORS.md,sha256=_nf9LY5n7wib7wT7oPRZqxRil0STaMq7JcvAwTph7tI,123
-elwood-0.1.1.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-elwood-0.1.1.dist-info/METADATA,sha256=p8KmhaI4FdWqBYvpUSrHdWtXmAEWNIymHSpnPdw536M,4943
-elwood-0.1.1.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-elwood-0.1.1.dist-info/entry_points.txt,sha256=TzJi2WjTTVW62q1YxjU0wNUn9F3QbPILW6A8VRe9Xes,43
-elwood-0.1.1.dist-info/top_level.txt,sha256=MKkVgr_DJlxlN-IlwnW98ogymP3HYNUDq7_aK-pftXg,7
-elwood-0.1.1.dist-info/RECORD,,
+elwood-0.1.2.dist-info/AUTHORS.md,sha256=_nf9LY5n7wib7wT7oPRZqxRil0STaMq7JcvAwTph7tI,123
+elwood-0.1.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+elwood-0.1.2.dist-info/METADATA,sha256=uuXgt-5tPPwhDx6EBJCzMvX5gzUbpeExr6z8V97wwo0,4943
+elwood-0.1.2.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
+elwood-0.1.2.dist-info/entry_points.txt,sha256=TzJi2WjTTVW62q1YxjU0wNUn9F3QbPILW6A8VRe9Xes,43
+elwood-0.1.2.dist-info/top_level.txt,sha256=MKkVgr_DJlxlN-IlwnW98ogymP3HYNUDq7_aK-pftXg,7
+elwood-0.1.2.dist-info/RECORD,,
```


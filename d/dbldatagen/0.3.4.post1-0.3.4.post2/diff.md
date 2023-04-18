# Comparing `tmp/dbldatagen-0.3.4.post1.tar.gz` & `tmp/dbldatagen-0.3.4.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbldatagen-0.3.4.post1.tar", last modified: Thu Apr 13 17:05:10 2023, max compression
+gzip compressed data, was "dbldatagen-0.3.4.post2.tar", last modified: Tue Apr 18 23:02:02 2023, max compression
```

## Comparing `dbldatagen-0.3.4.post1.tar` & `dbldatagen-0.3.4.post2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:05:10.222521 dbldatagen-0.3.4.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-04-13 17:05:10.222521 dbldatagen-0.3.4.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:05:10.218521 dbldatagen-0.3.4.post1/dbldatagen/
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    59147 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/column_generation_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/column_spec_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/data_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    57532 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/datagen_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/datarange.py
--rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/daterange.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:05:10.222521 dbldatagen-0.3.4.post1/dbldatagen/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/distributions/beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/distributions/data_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/distributions/exponential_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/distributions/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/distributions/normal_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/function_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/nrange.py
--rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/schema_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/spark_singleton.py
--rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/text_generator_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)    41986 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/text_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/dbldatagen/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 17:05:10.222521 dbldatagen-0.3.4.post1/dbldatagen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-04-13 17:05:10.000000 dbldatagen-0.3.4.post1/dbldatagen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-13 17:05:10.000000 dbldatagen-0.3.4.post1/dbldatagen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 17:05:10.000000 dbldatagen-0.3.4.post1/dbldatagen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-13 17:05:10.000000 dbldatagen-0.3.4.post1/dbldatagen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-13 17:05:10.222521 dbldatagen-0.3.4.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-13 17:03:33.000000 dbldatagen-0.3.4.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:02:02.265653 dbldatagen-0.3.4.post2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6327 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-04-18 23:02:02.265653 dbldatagen-0.3.4.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:02:02.265653 dbldatagen-0.3.4.post2/dbldatagen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59388 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/column_generation_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/column_spec_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/data_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57532 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/datagen_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/datarange.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7328 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/daterange.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:02:02.265653 dbldatagen-0.3.4.post2/dbldatagen/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/distributions/beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/distributions/data_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/distributions/exponential_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/distributions/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/distributions/normal_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/function_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/nrange.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15512 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/schema_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/spark_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15709 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/text_generator_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41986 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/text_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10827 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/dbldatagen/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 23:02:02.265653 dbldatagen-0.3.4.post2/dbldatagen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-04-18 23:02:02.000000 dbldatagen-0.3.4.post2/dbldatagen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-18 23:02:02.000000 dbldatagen-0.3.4.post2/dbldatagen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 23:02:02.000000 dbldatagen-0.3.4.post2/dbldatagen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 23:02:02.000000 dbldatagen-0.3.4.post2/dbldatagen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-18 23:02:02.265653 dbldatagen-0.3.4.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-18 23:00:15.000000 dbldatagen-0.3.4.post2/setup.py
```

### Comparing `dbldatagen-0.3.4.post1/CHANGELOG.md` & `dbldatagen-0.3.4.post2/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 # Databricks Labs Data Generator Release Notes
 
 ## Change History
 All notable changes to the Databricks Labs Data Generator will be documented in this file.
 
+### Version 0.3.4 Post 2
+
+### Fixed
+* Fix for use of values in columns of type array, map and struct 
+* Fix for generation of arrays via `numFeatures` and `structType` attributes when numFeatures has value of 1
+
+### Version 0.3.4 Post 1
+
+### Fixed
+* Fix for use and configuration of root logger 
+
+### Acknowledgements
+Thanks to Marvin Schenkel for the contribution
+
 ### Version 0.3.4
 
 #### Changed
 * Modified option to allow for range when specifying `numFeatures` with `structType='array'` to allow generation
   of varying number of columns
 * When generating multi-column or array valued columns, compute random seed with different name for each column
 * Additional build ordering enhancements to reduce circumstances where explicit base column must be specified
```

### Comparing `dbldatagen-0.3.4.post1/CONTRIBUTING.md` & `dbldatagen-0.3.4.post2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/LICENSE` & `dbldatagen-0.3.4.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/PKG-INFO` & `dbldatagen-0.3.4.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbldatagen
-Version: 0.3.4.post1
+Version: 0.3.4.post2
 Summary: Databricks Labs -  PySpark Synthetic Data Generator
 Home-page: https://github.com/databrickslabs/data-generator
 Author: Ronan Stokes, Databricks
 License: Databricks License
 Project-URL: Databricks Labs, https://www.databricks.com/learn/labs
 Project-URL: Documentation, https://databrickslabs.github.io/dbldatagen/public_docs/index.html
 Classifier: Programming Language :: Python :: 3
@@ -71,15 +71,15 @@
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
 can be found in the GitHub repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4post1/CHANGELOG.md)
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4post2/CHANGELOG.md)
 
 # Installation
 
 Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
```

### Comparing `dbldatagen-0.3.4.post1/PULL_REQUEST_TEMPLATE.md` & `dbldatagen-0.3.4.post2/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/README.md` & `dbldatagen-0.3.4.post2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
 can be found in the GitHub repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4post1/CHANGELOG.md)
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4post2/CHANGELOG.md)
 
 # Installation
 
 Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
```

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/__init__.py` & `dbldatagen-0.3.4.post2/dbldatagen/__init__.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/_version.py` & `dbldatagen-0.3.4.post2/dbldatagen/_version.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     major, minor, patch, release, build = r.match(version).groups()
     version_info = VersionInfo(major, minor, patch, release, build)
     logger = logging.getLogger(__name__)
     logger.info("Version : %s", version_info)
     return version_info
 
 
-__version__ = "0.3.4post1"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "0.3.4post2"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
 
 
 def _get_spark_version(sparkVersion):
     try:
         r = re.compile(r'(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>.*)')
         major, minor, patch, release = r.match(sparkVersion).groups()
```

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/column_generation_spec.py` & `dbldatagen-0.3.4.post2/dbldatagen/column_generation_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,14 +81,16 @@
 
     #: maxValue values for each column type, only if where value is intentionally restricted
     _max_type_range = {
         'byte': 256,
         'short': 65536
     }
 
+    _ARRAY_STRUCT_TYPE = "array"
+
     # set up logging
 
     # restrict spurious messages from java gateway
     logging.getLogger("py4j").setLevel(logging.WARNING)
 
     def __init__(self, name, colType=None, minValue=0, maxValue=None, step=1, prefix='', random=False,
                  distribution=None, baseColumn=None, randomSeed=None, randomSeedMethod=None,
@@ -1017,26 +1019,27 @@
             if type(self.datatype) is StringType and sformat is not None:
                 self.logger.warning("Formatting not supported for weighted columns")
                 self.executionHistory.append(".. WARNING: Formatting not supported for weighted columns")
         else:
             # rs: initialize the begin, end and interval if not initialized for date computations
             # defaults are start of day, now, and 1 minute respectively
 
-            if not type(self.datatype) in [ArrayType, MapType, StructType]:
+            # for array, struct and map types, either value is provided via `expr` or via values
+            if not type(self.datatype) in [ArrayType, MapType, StructType] or self.values is not None:
                 self._computeImpliedRangeIfNeeded(self.datatype)
 
             # TODO: add full support for date value generation
             if self.expr is not None:
                 # note use of SQL expression ignores range specifications
                 new_def = expr(self.expr).astype(self.datatype)
 
                 # record execution history
                 self.executionHistory.append(f".. using SQL expression `{self.expr}` as base")
                 self.executionHistory.append(f".. casting to  `{self.datatype}`")
-            elif type(self.datatype) in [ArrayType, MapType, StructType]:
+            elif type(self.datatype) in [ArrayType, MapType, StructType] and self.values is None:
                 new_def = expr("NULL")
             elif self._dataRange is not None and self._dataRange.isFullyPopulated():
                 self.executionHistory.append(f".. computing ranged value: {self._dataRange}")
                 new_def = self._computeRangedColumn(base_column=self.baseColumn, datarange=self._dataRange,
                                                     is_random=col_is_rand)
             elif type(self.datatype) is DateType:
                 # TODO: fixup for date generation
@@ -1200,15 +1203,15 @@
                 raise ValueError(f"Bad value [{num_columns}] for `numColumns` / `numFeatures` attribute")
         else:
             if validate:
                 raise ValueError(f"Bad value [{num_columns}] for `numColumns` / `numFeatures` attribute")
 
             min_num_columns, max_num_columns = 1, 1
 
-        if validate and (min_num_columns != max_num_columns) and (struct_type != "array"):
+        if validate and (min_num_columns != max_num_columns) and (struct_type != self._ARRAY_STRUCT_TYPE):
             self.logger.warning(
                 f"Varying number of features / columns specified for non-array column [{self.name}]")
             self.logger.warning(
                 f"Lower bound for number of features / columns ignored for [{self.name}]")
             min_num_columns = max_num_columns
 
         return min_num_columns, max_num_columns, struct_type
@@ -1224,15 +1227,15 @@
             :param self: is ColumnGenerationSpec for column
             :returns: spark sql `column` or expression that can be used to generate a column
         """
         min_num_columns, max_num_columns, struct_type = self._getMultiColumnDetails(validate=True)
 
         self.executionHistory = []
 
-        if (min_num_columns == 1) and (max_num_columns == 1):
+        if (min_num_columns == 1) and (max_num_columns == 1) and struct_type != self._ARRAY_STRUCT_TYPE:
             # record execution history for troubleshooting
             self.executionHistory.append(f"generating single column - `{self.name}` having type `{self.datatype}`")
 
             retval = self._makeSingleGenerationExpression(use_pandas_optimizations=True)
 
             # record how column was generated
             exec_step_history = ".. computed from base values - "
```

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/column_spec_options.py` & `dbldatagen-0.3.4.post2/dbldatagen/column_spec_options.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/data_analyzer.py` & `dbldatagen-0.3.4.post2/dbldatagen/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/data_generator.py` & `dbldatagen-0.3.4.post2/dbldatagen/data_generator.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/datagen_constants.py` & `dbldatagen-0.3.4.post2/dbldatagen/datagen_constants.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/datarange.py` & `dbldatagen-0.3.4.post2/dbldatagen/datarange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/daterange.py` & `dbldatagen-0.3.4.post2/dbldatagen/daterange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/distributions/__init__.py` & `dbldatagen-0.3.4.post2/dbldatagen/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/distributions/beta.py` & `dbldatagen-0.3.4.post2/dbldatagen/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/distributions/data_distribution.py` & `dbldatagen-0.3.4.post2/dbldatagen/distributions/data_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/distributions/exponential_distribution.py` & `dbldatagen-0.3.4.post2/dbldatagen/distributions/exponential_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/distributions/gamma.py` & `dbldatagen-0.3.4.post2/dbldatagen/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/distributions/normal_distribution.py` & `dbldatagen-0.3.4.post2/dbldatagen/distributions/normal_distribution.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/function_builder.py` & `dbldatagen-0.3.4.post2/dbldatagen/function_builder.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/nrange.py` & `dbldatagen-0.3.4.post2/dbldatagen/nrange.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/schema_parser.py` & `dbldatagen-0.3.4.post2/dbldatagen/schema_parser.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/spark_singleton.py` & `dbldatagen-0.3.4.post2/dbldatagen/spark_singleton.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/text_generator_plugins.py` & `dbldatagen-0.3.4.post2/dbldatagen/text_generator_plugins.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/text_generators.py` & `dbldatagen-0.3.4.post2/dbldatagen/text_generators.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen/utils.py` & `dbldatagen-0.3.4.post2/dbldatagen/utils.py`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/dbldatagen.egg-info/PKG-INFO` & `dbldatagen-0.3.4.post2/dbldatagen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbldatagen
-Version: 0.3.4.post1
+Version: 0.3.4.post2
 Summary: Databricks Labs -  PySpark Synthetic Data Generator
 Home-page: https://github.com/databrickslabs/data-generator
 Author: Ronan Stokes, Databricks
 License: Databricks License
 Project-URL: Databricks Labs, https://www.databricks.com/learn/labs
 Project-URL: Documentation, https://databrickslabs.github.io/dbldatagen/public_docs/index.html
 Classifier: Programming Language :: Python :: 3
@@ -71,15 +71,15 @@
 ## Documentation
 
 Please refer to the [online documentation](https://databrickslabs.github.io/dbldatagen/public_docs/index.html) for 
 details of use and many examples.
 
 Release notes and details of the latest changes for this specific release
 can be found in the GitHub repository
-[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4post1/CHANGELOG.md)
+[here](https://github.com/databrickslabs/dbldatagen/blob/release/v0.3.4post2/CHANGELOG.md)
 
 # Installation
 
 Use `pip install dbldatagen` to install the PyPi package.
 
 Within a Databricks notebook, invoke the following in a notebook cell
 ```commandline
```

### Comparing `dbldatagen-0.3.4.post1/dbldatagen.egg-info/SOURCES.txt` & `dbldatagen-0.3.4.post2/dbldatagen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbldatagen-0.3.4.post1/setup.py` & `dbldatagen-0.3.4.post2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     The Databricks Labs Data Generator can generate realistic synthetic data sets at scale for testing, 
     benchmarking, environment validation and other purposes.
     """
 
 setuptools.setup(
     name="dbldatagen",
-    version="0.3.4post1",
+    version="0.3.4post2",
     author="Ronan Stokes, Databricks",
     description="Databricks Labs -  PySpark Synthetic Data Generator",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/databrickslabs/data-generator",
     project_urls={
         "Databricks Labs": "https://www.databricks.com/learn/labs",
```

